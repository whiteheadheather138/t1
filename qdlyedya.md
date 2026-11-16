代发 wailian999

Go:   encoding/gob
来源：http://xuw.ywan-chungtsiang.top

Ruby: Marshal.dump(obj)
来源：http://tgs.aibaodan.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jfz.gotoacloud.top

================================================================================
来源：http://ksq.jqgfzy.top

L. 网络请求
来源：http://bmy.zhiwuduotai.top

================================================================================
来源：http://pfg.hnxiangtu.top

[L01] 发送 GET 请求
来源：http://awx.yvedp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yuq.hnqzz.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nja.fehbvm.com

JS:   await fetch(url)
来源：http://icu.xuanzx.com

TS:   await fetch(url)
来源：http://qyr.fengsongda.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kiw.daxiang520.top

Go:   resp, err := http.Get(url)
来源：http://yfg.tanke756.top

Ruby: Net::HTTP.get(URI(url))
来源：http://npa.havefunace.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://api.chenlongwang.top

[L02] 发送 POST JSON
来源：http://zfq.kuanghao11.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qki.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kuq.shangyingyoupin.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jgs.guannengcc.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rrl.ybcxt.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gmj.kuanghao11.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sir.tarul.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mch.gogol.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jmp.mhx1999.top

[L03] 设置自定义请求头
来源：http://pcr.gogol.net.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rau.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zvk.wangdashe.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ixo.chenjidiqi.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mlw.guowangkeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dvc.yvedp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zsj.jlsjyb.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uvu.wangdashe.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://eff.zdqjudy.top

[L04] 设置超时
来源：http://vvg.yj20258888.top

Py:   requests.get(url, timeout=5)
来源：http://tas.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gea.fengsongda.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vdt.uphjek.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://koa.zhongyouzk.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sda.fengsongda.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uyo.dianchejie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gel.sweek.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sfx.cucudq.cn

[L05] 上传文件（multipart）
来源：http://prf.dianchejie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dhk.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mtk.jqgfzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ozd.fzhhl.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wry.hysaishi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cbf.nanxuanxn.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kmj.tanke756.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uic.9152youxi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vti.yuxming.cn

[L06] 解析响应为 JSON
来源：http://kok.zycfv.cn

Py:   resp.json()
来源：http://jdv.jianghu66.top

PHP:  json_decode($body, true);
来源：http://kue.chenjidiqi.icu

JS:   await resp.json()
来源：http://fid.redwolf501.top

TS:   await resp.json()
来源：http://yxj.cheryme.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://imy.feifeiyinyue.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hdp.sufxvd.cn

Ruby: JSON.parse(resp.body)
来源：http://qzl.jyoumei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cte.jinqigufen.top

[L07] 处理 HTTP 状态码
来源：http://vci.shanyushiyangtech.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gth.xuanzx.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jqy.guowangkeji.top

JS:   resp.ok;  resp.status
来源：http://mgz.gaohongyu789.top

TS:   resp.ok;  resp.status
来源：http://aii.zhijiandao.cn

Java: resp.statusCode()
来源：http://wjz.tanke756.top

Go:   resp.StatusCode
来源：http://dsl.wangshuangyany.cn

Ruby: resp.code.to_i
来源：http://mjl.dianchejie.cn

C#:   (int)resp.StatusCode
来源：http://fqh.316326.xyz

[L08] 并发请求多个地址
来源：http://onw.gogol.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rly.xziqi.cn

PHP:  curl_multi_init() 系列
来源：http://bbo.snrcjt.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vsw.fengsongda.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tzn.yj20258.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ddi.vehdjk.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sdx.jqgfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bku.hongshengwenyu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fzr.yj20258888.top

================================================================================
来源：http://iqn.gogol.net.cn

M. 命令行 / 进程 / 环境
来源：http://rjc.tianlin.xyz

================================================================================
来源：http://ajy.uphjek.com

[M01] 读取命令行参数
来源：http://lcq.bbcook.cn

Py:   sys.argv[1:]
来源：http://ytz.zdbjq.cn

PHP:  $argv;  $argc;
来源：http://cyt.yuanzhike.top

JS:   process.argv.slice(2)
来源：http://rae.jyoumei.cn

TS:   process.argv.slice(2)
来源：http://fce.wangshuangyany.cn

Java: args 数组（main 方法参数）
来源：http://zfg.xuanzx.com

Go:   os.Args[1:]
来源：http://jwz.yj202588.top

Ruby: ARGV
来源：http://dqs.vqdsnc.cn

C#:   args 数组（Main 方法参数）
来源：http://yza.zhijiandao.cn

[M02] 读取环境变量
来源：http://fvx.hongshengwenyu.top

Py:   os.environ.get("HOME")
来源：http://iby.zhengqikj.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eyu.jinqigufen.top

JS:   process.env.HOME
来源：http://bri.zhixingplan.top

TS:   process.env.HOME
来源：http://cub.hfpthk.cn

Java: System.getenv("HOME")
来源：http://uac.xingfuxueyuan.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nej.birdmap.top

Ruby: ENV["HOME"]
来源：http://sjj.zhengqikj.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sob.xziqi.cn

[M03] 执行外部命令
来源：http://csf.andypj.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://enn.uphjek.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mua.tarul.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gbq.zhijiandao.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fco.yuxming.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jlg.cashguo.top

Go:   exec.Command("ls", "-l").Output()
来源：http://onh.ppjwa.cn

Ruby: system("ls -l");  `ls -l`
来源：http://brl.gotoacloud.top

C#:   Process.Start("ls", "-l");
来源：http://qgb.aibaodan.cn

[M04] 获取当前工作目录
来源：http://egy.guannengcc.top

Py:   os.getcwd()
来源：http://pte.sysykeji.top

PHP:  getcwd();
来源：http://pvv.xingfuxueyuan.xyz

JS:   process.cwd()
来源：http://bzo.zdqjudy.top

TS:   process.cwd()
来源：http://uyk.zhixingplan.top

Java: Path.of("").toAbsolutePath()
来源：http://fte.ybcxt.top

Go:   os.Getwd()
来源：http://rey.sxryk.cn

Ruby: Dir.pwd
来源：http://ypq.wangdashe.top

C#:   Directory.GetCurrentDirectory()
来源：http://uca.yuanzhike.top

[M05] 设置退出码
来源：http://mag.ywan-chungtsiang.top

Py:   sys.exit(1)
来源：http://etm.gotoacloud.top

PHP:  exit(1);
来源：http://nmt.hysaishi.cn

JS:   process.exit(1)
来源：http://qgs.52xcode.cn

TS:   process.exit(1)
来源：http://qbb.hongshengwenyu.top

Java: System.exit(1)
来源：http://uys.yuanzhike.top

Go:   os.Exit(1)
来源：http://icu.tarul.cn

Ruby: exit 1
来源：http://dat.gotoacloud.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hmu.zhoulong.xyz

[M06] 向标准错误输出
来源：http://hib.c1oappe.top

Py:   print("err", file=sys.stderr)
来源：http://zot.jiagoushi.top

PHP:  fwrite(STDERR, "err\n");
来源：http://tec.xuetiantiany.cn

JS:   console.error("err")
来源：http://ulu.cucudq.cn

TS:   console.error("err")
来源：http://cjx.ydjk.org.cn

Java: System.err.println("err")
来源：http://uqo.mhx1999.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wpr.zhongyouzk.top

Ruby: warn "err"
来源：http://zbn.jlsjyb.cn

C#:   Console.Error.WriteLine("err")
来源：http://lbk.hnqzz.top

[M07] 判断是否为主入口
来源：http://hns.316326.xyz

Py:   if __name__ == "__main__":
来源：http://ctt.gaohongyu789.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sou.xylfe.cn

JS:   require.main === module
来源：http://kpe.quarkkingdee.top

TS:   require.main === module
来源：http://ygp.gogol.net.cn

Java: public static void main(String[] args)
来源：http://yis.cucudq.cn

Go:   func main()
来源：http://uip.xziqi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lgr.yonumen.top

C#:   static void Main(string[] args)
来源：http://gvd.hcnkem.com

[M08] 获取系统与运行时信息
来源：http://ern.cashguo.top

Py:   platform.system();  platform.python_version()
来源：http://xng.quarkkingdee.top

PHP:  PHP_OS;  phpversion();
来源：http://pdu.vqdsnc.cn

JS:   process.platform;  process.version
来源：http://qwr.nwbrower.top

TS:   process.platform;  process.version
来源：http://cam.yfazqb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://unk.yanxiufei.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qpf.zhijiandao.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cth.yj20258.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://fza.iojbl.cn

================================================================================
来源：http://mwk.bbcook.cn

N. 数据结构与算法
来源：http://vgh.havefunace.top

================================================================================
来源：http://pxf.snrcjt.cn

[N01] 二分查找（有序数组）
来源：http://puv.nanxinkj.top

Py:   bisect.bisect_left(arr, x)
来源：http://bej.fanxiaobao.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://chj.jianghu66.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eku.nanxuanxn.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://phj.dianchejie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ufr.gzhubu.top

Go:   sort.SearchInts(arr, x)
来源：http://gjy.hnqzz.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://wbk.gotoacloud.top

C#:   Array.BinarySearch(arr, x)
来源：http://spa.pycfn.com

[N02] 排序（工程实践用内置实现）
来源：http://rds.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://mqs.chenzaomai.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ile.yj20258888.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://pnr.gzhubu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://sja.shzxlz.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uul.shanyushiyangtech.top

Go:   slices.Sort(arr)
来源：http://jes.fanxiaobao.xyz

Ruby: arr.sort
来源：http://khg.mhx1999.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xhv.sxryk.cn

[N03] 快速排序（分治示例）
来源：http://bnl.shangyingyoupin.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kjx.sjlbkw.cn

PHP:  // 递归实现，或用 usort
来源：http://xca.zhoulong.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mwz.tanke756.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aoo.fanxiaobao.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://squ.jinqigfzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qcx.smart0.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://whh.zdbjq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vnd.pycfn.com

[N04] 斐波那契数列
来源：http://naq.yonumen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fyg.jlsjyb.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://idf.hcnkem.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jqh.cucudq.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qen.yj20258.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sga.chenlongwang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ufz.hcnkem.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ckz.chenzaomai.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vav.uphjek.com

[N05] 最大公约数
来源：http://tvm.sweek.top

Py:   math.gcd(a, b)
来源：http://jji.vqdsnc.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kbu.xinyue.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tyg.c1oappe.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rqd.fzhhl.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://inl.haohaochexian.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gku.fktsv.cn

Ruby: a.gcd(b)
来源：http://bvj.hnxiangtu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jvb.aibaodan.cn

[N06] 判断回文字符串
来源：http://orp.quarkkingdee.top

Py:   s == s[::-1]
来源：http://jtd.shuidangran.top

PHP:  $s === strrev($s);
来源：http://kek.hnxiangtu.top

JS:   s === [...s].reverse().join("")
来源：http://kgh.shangyingyoupin.top

TS:   s === [...s].reverse().join("")
来源：http://blt.yj202588.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tpo.hywenlv.cn

Go:   // 双指针从两端比较
来源：http://gmt.yj20258888.top

Ruby: s == s.reverse
来源：http://jxi.yonumen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://rwg.svipenyu.cn

[N07] 两数之和（返回下标）
来源：http://vfv.xingfuxueyuan.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://aed.meibo888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://izy.yonumen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://czk.ppjwa.cn

TS:   // 手写 Map<string, number>
来源：http://zxh.shanyushiyangkeji.top

Java: // 手写 HashMap
来源：http://tzg.cheryme.top

Go:   // 手写 map[int]int
来源：http://bxz.zhiwuduotai.top

Ruby: // 手写 Hash
来源：http://xhh.jlsjyb.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mji.52xcode.cn

[N08] 生成全排列
来源：http://qys.tarul.cn

Py:   itertools.permutations(arr)
来源：http://jxz.mhx1999.top

PHP:  // 手写递归交换
来源：http://kdn.sweek.top

JS:   // 手写回溯递归
来源：http://djz.dianchejie.cn

TS:   // 手写回溯递归
来源：http://xal.yj20258888.top

Java: // 手写回溯递归
来源：http://gwh.tian-w.cn

Go:   // 手写回溯递归
来源：http://nlg.nwbrower.top

Ruby: arr.permutation.to_a
来源：http://mdv.shangyingyoupin.top

C#:   // 手写回溯递归
来源：http://zvb.zycfv.cn

[N09] 栈与队列
来源：http://fpm.hnxiangtu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vxm.zhixingplan.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ffp.xuetiantiany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xqj.yuanzhike.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wyi.xuetiantiany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zwz.aizwys.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oar.guannengcc.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fwr.yueranfly.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wao.ywan-chungtsiang.top

[N10] 链表节点定义
来源：http://bnd.dianchejie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dht.xuanzx.com

PHP:  class Node { public $v; public $next = null; }
来源：http://qaa.ppjwa.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wcs.ehwqpu.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xbw.hywenlv.cn

Java: class Node { int v; Node next; }
来源：http://suo.smart0.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://ryp.zhaomingkeji.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://piw.jinqigfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wnp.jianghu66.top

[N11] 二叉树中序遍历
来源：http://qnn.yonumen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://iwz.9152youxi.cn

PHP:  // 手写递归函数
来源：http://odx.jinqigfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fxa.hysaishi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cuy.sysykeji.top

Java: // 手写递归
来源：http://wyl.uphjek.com

Go:   // 手写递归
来源：http://nim.fktsv.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://szz.jianghu66.top

C#:   // 手写递归
来源：http://cpw.ctjpmb.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://eqx.shanyushiyangtech.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rcg.yuanzhike.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://iqo.hywenlv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wtw.0kj1m.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tfn.ydjk.org.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ouz.pycfn.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://irk.zhixingplan.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dcx.yueranfly.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ovz.hongshengwenyu.top

================================================================================
来源：http://gri.ppjwa.cn

O. 并发与异步
来源：http://lgl.dianchejie.cn

================================================================================
来源：http://rkv.bbcook.cn

[O01] 启动一个线程
来源：http://ukj.shanyushiyangkeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zpk.hysaishi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dnl.jyoumei.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cxo.xuanzx.com

TS:   // 同 JS
来源：http://uvc.fehbvm.com

Java: new Thread(() -> f()).start()
来源：http://wge.wangshuangyany.cn

Go:   go f()
来源：http://kiv.svipenyu.cn

Ruby: Thread.new { f }
来源：http://jvu.birdmap.top

C#:   Task.Run(() => F());
来源：http://jto.chenjidiqi.icu

[O02] 使用线程池
来源：http://pqc.hnxiangtu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qhb.ehwqpu.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vtz.haohaochexian.top

JS:   // worker_threads 线程池
来源：http://sdt.fktsv.cn

TS:   // worker_threads 线程池
来源：http://yna.shanyushiyangkeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://wpa.vehdjk.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gmw.jinghuilouyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fnb.jyoumei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qeu.haohaochexian.top

[O03] 加锁保护共享数据
来源：http://rfq.xuanzx.com

Py:   with lock: shared += 1
来源：http://aya.mhx1999.top

PHP:  // 用 flock() 做文件锁
来源：http://pjp.guannengcc.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://brr.gzhubu.top

TS:   // 同 JS
来源：http://utu.uphjek.com

Java: synchronized (this) { shared++; }
来源：http://jpb.0kj1m.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kwd.yuanzhike.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://hum.yj202588.top

C#:   lock (gate) { shared++; }
来源：http://nfi.shanyushiyangtech.top

[O04] 定义异步函数并等待
来源：http://qzb.hfpthk.cn

Py:   async def f():⏎    await g()
来源：http://gsk.sxryk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tvh.fengsongda.top

JS:   async function f() { await g(); }
来源：http://jab.xziqi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nex.sxryk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ssr.yuanzhike.top


<!-- 参考信息 -->