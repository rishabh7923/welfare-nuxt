<template>
    <main>
        <Header />
        <div class="container mt-3">
            <h1 class="heading">BAL MELA</h1>
            <div class="divider"><span></span></div>

            <div class="row">
                <div class="col-md-8 mb-2">
                    <b-skeleton-wrapper :loading="loading">
                        <template #loading>
                            <b-skeleton-img no-aspect height="30rem"></b-skeleton-img>
                        </template>
                        <iframe
                            class="embed-responsive-item w-100 rounded h-100 animate slide"
                            src="https://www.youtube.com/embed/jpQi9T-SWaY?rel=0&modestbranding=1&autohide=1&mute=1&showinfo=0&controls=1&autoplay=1&playlist=jpQi9T-SWaY&loop=1&start=9"
                            allowfullscreen>
                        </iframe> 
                    </b-skeleton-wrapper>
                </div>

                <div class="col bg-stylish rounded">
                    <h3 class="heading mt-2">What is it?</h3>
                    <div class="divider mb-1"><span></span></div>

                    <p>
                        Over the past many years school has been organizing The Grand Bal Mela which is a Charity
                        Fundraiser. It has become a successful fun-filled event. The students of classes ninth to
                        twelfth
                        take lead in calculating the budget, organizing, marketing, publicity and managing the
                        profitability.
                    </p>

                    <p>
                        By organizing such events the school provides the students to learn the very important
                        attributes of cooperation, teamwork, entrepreneurship, leadership, and most importantly social
                        service because every profit that they make is donated for a special cause. Overall it is an
                        overwhelming experience and a major learning opportunity for all students.
                    </p>
                </div>
            </div>

        </div>
        <Footer />
    </main>
</template>

<script>
export default {
    data() {
        return { 
            loading: true
        }
    },

    mounted() {
        setTimeout(() => this.loading = false, 500)
    }
}
</script>