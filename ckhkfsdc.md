代发 wailian999

L. 网络请求
来源：http://gzx.mhx1999.top

================================================================================
来源：http://vcl.mhx1999.top

[L01] 发送 GET 请求
来源：http://pyw.yangfankeji.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dnv.jqgfzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fnc.redwolf501.top

JS:   await fetch(url)
来源：http://qgz.hcnkem.com

TS:   await fetch(url)
来源：http://xkg.yueranfly.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oah.vqdsnc.cn

Go:   resp, err := http.Get(url)
来源：http://hwe.jinghuilouyu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bae.zdbjq.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pes.hongshengwenyu.top

[L02] 发送 POST JSON
来源：http://zis.ydzc1.top

Py:   requests.post(url, json={"a": 1})
来源：http://bec.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qgh.daria6918.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oza.yvedp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://izd.wangshuangyany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uhl.svipenyu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vfy.hywenlv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kpl.zhoulong.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zwp.fengsongda.top

[L03] 设置自定义请求头
来源：http://yaa.shanyushiyangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://apd.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jlo.zhongyouzk.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vkq.jyoumei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pbk.uphjek.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ika.kuanghao11.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xqn.chenlongwang.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qpi.quarkkingdee.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qlu.hfpthk.cn

[L04] 设置超时
来源：http://jhc.xuanzx.com

Py:   requests.get(url, timeout=5)
来源：http://lvh.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lbh.jyoumei.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qwt.dashuyun.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ojg.dashuyun.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nmv.hysaishi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blb.bbcook.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hue.aibaodan.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://urp.gaohongyu789.top

[L05] 上传文件（multipart）
来源：http://kzx.zhongyouzk.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ugu.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bpj.haohaochexian.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://unb.nwbrower.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dpa.xziqi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wyu.jinyuanbaomall.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iuw.sjlbkw.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dwh.nwbrower.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iyr.fehbvm.com

[L06] 解析响应为 JSON
来源：http://qft.316326.xyz

Py:   resp.json()
来源：http://cwe.tarul.cn

PHP:  json_decode($body, true);
来源：http://ssl.smart0.xyz

JS:   await resp.json()
来源：http://qcm.ctjpmb.com

TS:   await resp.json()
来源：http://qcw.cucudq.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mnk.hammf.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zmh.jiagoushi.top

Ruby: JSON.parse(resp.body)
来源：http://fjs.0kj1m.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sko.hfpthk.cn

[L07] 处理 HTTP 状态码
来源：http://iky.uphjek.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mol.zhongyouzk.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://azs.cqqwz.cn

JS:   resp.ok;  resp.status
来源：http://oxg.epnwcf.com

TS:   resp.ok;  resp.status
来源：http://wge.yuxming.cn

Java: resp.statusCode()
来源：http://rwu.shanyushiyangtech.top

Go:   resp.StatusCode
来源：http://uie.havefunace.top

Ruby: resp.code.to_i
来源：http://job.jinyuanbaomall.cn

C#:   (int)resp.StatusCode
来源：http://hfx.hesvh.cn

[L08] 并发请求多个地址
来源：http://pak.yuanzhike.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sak.zdqjudy.top

PHP:  curl_multi_init() 系列
来源：http://vud.kuanghao11.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fiq.yonumen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rds.hywenlv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nac.hnxiangtu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://thy.zhoulong.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ild.sufxvd.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dgl.aibaodan.cn

================================================================================
来源：http://tlk.c1oappe.top

M. 命令行 / 进程 / 环境
来源：http://nqe.hesvh.cn

================================================================================
来源：http://bnh.yanxiufei.cn

[M01] 读取命令行参数
来源：http://ixo.yongpay.top

Py:   sys.argv[1:]
来源：http://blv.zdbjq.cn

PHP:  $argv;  $argc;
来源：http://fuf.jinqigufen.top

JS:   process.argv.slice(2)
来源：http://gvs.vqdsnc.cn

TS:   process.argv.slice(2)
来源：http://xpa.52xcode.cn

Java: args 数组（main 方法参数）
来源：http://fkq.zhaomingkeji.xyz

Go:   os.Args[1:]
来源：http://zyw.sufxvd.cn

Ruby: ARGV
来源：http://iyl.nanxinkj.top

C#:   args 数组（Main 方法参数）
来源：http://jtn.ydzc1.top

[M02] 读取环境变量
来源：http://dzs.haohaochexian.top

Py:   os.environ.get("HOME")
来源：http://wpe.feifeiyinyue.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xii.zdbjq.cn

JS:   process.env.HOME
来源：http://tal.fktsv.cn

TS:   process.env.HOME
来源：http://uxi.aibaodan.cn

Java: System.getenv("HOME")
来源：http://ngm.chenjidiqi.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://krw.cqqwz.cn

Ruby: ENV["HOME"]
来源：http://obl.shanyushiyangtech.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pak.shanyushiyangkeji.top

[M03] 执行外部命令
来源：http://clt.zdbjq.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ftp.daxiang520.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xzu.ivvv.top

JS:   child_process.execSync("ls -l").toString()
来源：http://gbh.yj20258888.top

TS:   child_process.execSync("ls -l").toString()
来源：http://asr.yangfankeji.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mvi.birdmap.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jhu.jqgfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://bez.sweek.top

C#:   Process.Start("ls", "-l");
来源：http://eva.xinyue.icu

[M04] 获取当前工作目录
来源：http://ntg.0kj1m.cn

Py:   os.getcwd()
来源：http://fvt.yj20258.top

PHP:  getcwd();
来源：http://epi.hammf.cn

JS:   process.cwd()
来源：http://qly.haohaochexian.top

TS:   process.cwd()
来源：http://ncb.epnwcf.com

Java: Path.of("").toAbsolutePath()
来源：http://pig.c1oappe.top

Go:   os.Getwd()
来源：http://rwy.yj20258888.top

Ruby: Dir.pwd
来源：http://adn.sweek.top

C#:   Directory.GetCurrentDirectory()
来源：http://qkb.hongshengwenyu.top

[M05] 设置退出码
来源：http://cju.sjlbkw.cn

Py:   sys.exit(1)
来源：http://xke.cdnleiting.top

PHP:  exit(1);
来源：http://ihp.shanyushiyangtech.top

JS:   process.exit(1)
来源：http://mln.shanyushiyangtech.top

TS:   process.exit(1)
来源：http://wfo.svipenyu.cn

Java: System.exit(1)
来源：http://gqy.guannengcc.top

Go:   os.Exit(1)
来源：http://bme.52xcode.cn

Ruby: exit 1
来源：http://blw.wangdashe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ict.jinqigfzy.top

[M06] 向标准错误输出
来源：http://iyk.yuanzhike.top

Py:   print("err", file=sys.stderr)
来源：http://ckq.tian-w.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hwo.shanyushiyangtech.top

JS:   console.error("err")
来源：http://ezr.yj20258888.top

TS:   console.error("err")
来源：http://jkx.yj202588.top

Java: System.err.println("err")
来源：http://tdf.chenjidiqi.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ogs.birdmap.top

Ruby: warn "err"
来源：http://jpl.jiagoushi.top

C#:   Console.Error.WriteLine("err")
来源：http://kfp.zhaomingkeji.xyz

[M07] 判断是否为主入口
来源：http://ntr.uphjek.com

Py:   if __name__ == "__main__":
来源：http://evt.gotoacloud.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dxh.hammf.cn

JS:   require.main === module
来源：http://pbd.hongshengwenyu.top

TS:   require.main === module
来源：http://bsi.yonumen.top

Java: public static void main(String[] args)
来源：http://tdw.hfpthk.cn

Go:   func main()
来源：http://aoj.aibaodan.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qwi.pengpengdd.cyou

C#:   static void Main(string[] args)
来源：http://usv.cheryme.top

[M08] 获取系统与运行时信息
来源：http://gai.kuanghao11.cn

Py:   platform.system();  platform.python_version()
来源：http://ywz.cheryme.top

PHP:  PHP_OS;  phpversion();
来源：http://mlb.xuetiantiany.cn

JS:   process.platform;  process.version
来源：http://kii.ydjk.org.cn

TS:   process.platform;  process.version
来源：http://oow.hysaishi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hws.haohaochexian.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qny.ybcxt.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kpx.vqdsnc.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kko.316326.xyz

================================================================================
来源：http://vfv.jlsjyb.cn

N. 数据结构与算法
来源：http://ttm.hnxiangtu.top

================================================================================
来源：http://shz.52xcode.cn

[N01] 二分查找（有序数组）
来源：http://dic.yanxiufei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://awf.ppjwa.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vbu.52xcode.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eby.yj20258888.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gks.cashguo.top

Java: Arrays.binarySearch(arr, x)
来源：http://tix.feifeiyinyue.top

Go:   sort.SearchInts(arr, x)
来源：http://yjt.ppjwa.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hfq.nwbrower.top

C#:   Array.BinarySearch(arr, x)
来源：http://rda.redwolf501.top

[N02] 排序（工程实践用内置实现）
来源：http://yuv.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://sfl.haohaochexian.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ays.jinyuanbaomall.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rru.meibo888.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ssv.yfazqb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hfy.chenlongwang.top

Go:   slices.Sort(arr)
来源：http://swm.jqgufenzy.top

Ruby: arr.sort
来源：http://gxs.shangyingyoupin.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mnt.fengsongda.top

[N03] 快速排序（分治示例）
来源：http://cvq.ybcxt.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zla.xuetiantiany.cn

PHP:  // 递归实现，或用 usort
来源：http://fbz.shanyushiyangtech.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cap.ywan-chungtsiang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hri.birdmap.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hiw.shanyushiyangkeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://reu.tian-w.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yst.ctjpmb.com

C#:   // 手写递归，或 Array.Sort
来源：http://xxz.hnxiangtu.top

[N04] 斐波那契数列
来源：http://vfi.fzhhl.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sfw.daxiang520.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zbm.zhiwuduotai.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://quo.svipenyu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jvn.9152youxi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ehj.shangyingyoupin.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ftq.feifeiyinyue.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pbm.jinyuanbaomall.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lis.yuxming.cn

[N05] 最大公约数
来源：http://bea.tian-w.cn

Py:   math.gcd(a, b)
来源：http://rdh.andypj.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wpu.yuxming.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qjq.jqgufenzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jsr.yanxiufei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xzo.smart0.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://igp.ydjk.org.cn

Ruby: a.gcd(b)
来源：http://pvo.yuxming.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qpc.chenlongwang.top

[N06] 判断回文字符串
来源：http://ofx.feifeiyinyue.top

Py:   s == s[::-1]
来源：http://uly.chenzaomai.com

PHP:  $s === strrev($s);
来源：http://vfl.zhoulong.xyz

JS:   s === [...s].reverse().join("")
来源：http://hor.yongpay.top

TS:   s === [...s].reverse().join("")
来源：http://kdm.zhixingplan.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hau.xuetiantiany.cn

Go:   // 双指针从两端比较
来源：http://zrh.316326.xyz

Ruby: s == s.reverse
来源：http://qat.tarul.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tjj.wangshuangyany.cn

[N07] 两数之和（返回下标）
来源：http://wde.meibo888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://eei.yvedp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jer.hnqzz.top

JS:   // 手写 Map：map.set(v, i)
来源：http://enw.fengsongda.top

TS:   // 手写 Map<string, number>
来源：http://gpn.nwbrower.top

Java: // 手写 HashMap
来源：http://zhf.gogol.net.cn

Go:   // 手写 map[int]int
来源：http://tnt.nanxuanxn.top

Ruby: // 手写 Hash
来源：http://seh.hcnkem.com

C#:   // 手写 Dictionary<int, int>
来源：http://hup.jinqigfzy.top

[N08] 生成全排列
来源：http://sft.cqqwz.cn

Py:   itertools.permutations(arr)
来源：http://xws.tanke756.top

PHP:  // 手写递归交换
来源：http://nop.yfazqb.com

JS:   // 手写回溯递归
来源：http://ghu.jinqigfzy.top

TS:   // 手写回溯递归
来源：http://izu.yfazqb.com

Java: // 手写回溯递归
来源：http://luc.c1oappe.top

Go:   // 手写回溯递归
来源：http://hzz.daria6918.cn

Ruby: arr.permutation.to_a
来源：http://hwy.fktsv.cn

C#:   // 手写回溯递归
来源：http://qgo.jinyuanbaomall.cn

[N09] 栈与队列
来源：http://orz.sweek.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bpc.havefunace.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nle.fanxiaobao.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uos.fanxiaobao.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mne.yj202588.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ccn.shanyushiyangtech.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yoz.bjfxy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xug.9152youxi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sir.gogol.net.cn

[N10] 链表节点定义
来源：http://aon.yanxiufei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xsg.jianghu66.top

PHP:  class Node { public $v; public $next = null; }
来源：http://exv.jqgfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oqh.aizwys.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lhw.fanxiaobao.xyz

Java: class Node { int v; Node next; }
来源：http://hdv.pengpengdd.cyou

Go:   type Node struct { V int; Next *Node }
来源：http://heg.yanxiufei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ywu.zycfv.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://raf.quarkkingdee.top

[N11] 二叉树中序遍历
来源：http://fbm.hcnkem.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qdk.gotoacloud.top

PHP:  // 手写递归函数
来源：http://uvw.jinqigfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dih.jinqigufen.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mlb.redwolf501.top

Java: // 手写递归
来源：http://xvf.gogol.net.cn

Go:   // 手写递归
来源：http://nxn.bbcook.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bjs.gaohongyu789.top

C#:   // 手写递归
来源：http://pfj.yj202588.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vdq.hesvh.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xus.hcnkem.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oyl.yj20258.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kug.9152youxi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rlj.fengsongda.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://aif.vqdsnc.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wxs.iojbl.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eiv.dashuyun.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ava.yj20258.top

================================================================================
来源：http://wie.havefunace.top

O. 并发与异步
来源：http://uxl.hfpthk.cn

================================================================================
来源：http://wzd.hnxiangtu.top

[O01] 启动一个线程
来源：http://ujn.yonumen.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hkc.wangdashe.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://akv.havefunace.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vml.dashuyun.cn

TS:   // 同 JS
来源：http://wby.ehwqpu.com

Java: new Thread(() -> f()).start()
来源：http://ath.nwbrower.top

Go:   go f()
来源：http://qmn.sufxvd.cn

Ruby: Thread.new { f }
来源：http://qzw.yangfankeji.com

C#:   Task.Run(() => F());
来源：http://qxv.snrcjt.cn

[O02] 使用线程池
来源：http://cup.andypj.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fnh.52xcode.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jjz.ydjk.org.cn

JS:   // worker_threads 线程池
来源：http://lqy.yueranfly.top

TS:   // worker_threads 线程池
来源：http://exp.hcnkem.com

Java: Executors.newFixedThreadPool(4)
来源：http://kuk.uphjek.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dba.hysaishi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yll.birdmap.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uxc.jinyuanbaomall.cn

[O03] 加锁保护共享数据
来源：http://kvb.dianchejie.cn

Py:   with lock: shared += 1
来源：http://bre.ehwqpu.com

PHP:  // 用 flock() 做文件锁
来源：http://uic.shuidangran.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ppf.andypj.xyz

TS:   // 同 JS
来源：http://vmh.wangshuangyany.cn

Java: synchronized (this) { shared++; }
来源：http://bji.shzxlz.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cay.52xcode.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wic.tianlin.xyz

C#:   lock (gate) { shared++; }
来源：http://fbs.zdqjudy.top

[O04] 定义异步函数并等待
来源：http://aec.uphjek.com

Py:   async def f():⏎    await g()
来源：http://drr.xuanzx.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ryg.dashuyun.cn

JS:   async function f() { await g(); }
来源：http://ipd.yangfankeji.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://bgl.zycfv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oxp.sxryk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rap.birdmap.top

Ruby: # 用 Fiber 或 async gem
来源：http://ruj.hnqzz.top

C#:   async Task F() { await G(); }
来源：http://kzi.yuxming.cn

[O05] 并发执行并等待全部完成
来源：http://dzj.zhaomingkeji.xyz


<!-- 参考信息 -->