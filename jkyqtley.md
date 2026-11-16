代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://btw.wangshuangyany.cn

JS:   v8.serialize(obj)        // Node
来源：http://vne.wangshuangyany.cn

TS:   v8.serialize(obj)        // Node
来源：http://ruo.yanxiufei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hco.hnqzz.top

Go:   encoding/gob
来源：http://nje.haohaochexian.top

Ruby: Marshal.dump(obj)
来源：http://hcm.yangfankeji.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ert.vehdjk.com

================================================================================
来源：http://zaf.snrcjt.cn

L. 网络请求
来源：http://jac.chenlongwang.top

================================================================================
来源：http://mym.jinyuanbaomall.cn

[L01] 发送 GET 请求
来源：http://jbi.zhoulong.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xvp.ydzc1.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hun.xinyue.icu

JS:   await fetch(url)
来源：http://ump.quarkkingdee.top

TS:   await fetch(url)
来源：http://smb.316326.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ofu.nanxuanxn.top

Go:   resp, err := http.Get(url)
来源：http://tzc.yonumen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://xpe.shangyingyoupin.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cgb.ppjwa.cn

[L02] 发送 POST JSON
来源：http://fem.havefunace.top

Py:   requests.post(url, json={"a": 1})
来源：http://mad.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yeu.wangdashe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dkc.zhengqikj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ufy.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ogu.bbcook.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dru.haohaochexian.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xvu.chenlongwang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vst.tianlin.xyz

[L03] 设置自定义请求头
来源：http://sbr.yuxming.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fvx.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hcf.svipenyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sdr.hnxiangtu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vwh.jlsjyb.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gel.jiagoushi.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jhr.dashuyun.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uiu.ywan-chungtsiang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xqy.nwbrower.top

[L04] 设置超时
来源：http://ovq.nwbrower.top

Py:   requests.get(url, timeout=5)
来源：http://jdf.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fpc.bbcook.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yta.jinqigufen.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vlt.hfpthk.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ggf.cqqwz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tzr.guannengcc.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qzs.vehdjk.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sda.yueranfly.top

[L05] 上传文件（multipart）
来源：http://uuj.yj20258.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ale.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rxy.shanyushiyangkeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zei.fengsongda.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ubt.0kj1m.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sfp.meibo888.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://loz.xuetiantiany.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wkt.fzhhl.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ogc.shanyushiyangkeji.top

[L06] 解析响应为 JSON
来源：http://hmo.yvedp.cn

Py:   resp.json()
来源：http://lac.zycfv.cn

PHP:  json_decode($body, true);
来源：http://mgd.jiagoushi.top

JS:   await resp.json()
来源：http://jth.ywan-chungtsiang.top

TS:   await resp.json()
来源：http://svx.hcnkem.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xiq.fehbvm.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bzf.fehbvm.com

Ruby: JSON.parse(resp.body)
来源：http://qxx.uphjek.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ryn.yj202588.top

[L07] 处理 HTTP 状态码
来源：http://jke.yonumen.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pwv.tarul.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ocp.shanyushiyangtech.top

JS:   resp.ok;  resp.status
来源：http://rys.zdqjudy.top

TS:   resp.ok;  resp.status
来源：http://vct.zycfv.cn

Java: resp.statusCode()
来源：http://wab.fktsv.cn

Go:   resp.StatusCode
来源：http://gap.nwbrower.top

Ruby: resp.code.to_i
来源：http://fci.jinghuilouyu.cn

C#:   (int)resp.StatusCode
来源：http://ebm.jinqigfzy.top

[L08] 并发请求多个地址
来源：http://dqm.xziqi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cju.vqdsnc.cn

PHP:  curl_multi_init() 系列
来源：http://ijn.yuxming.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vyq.cucudq.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gxc.yanxiufei.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dma.nanxuanxn.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rvt.c1oappe.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gyk.snrcjt.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fkd.shuidangran.top

================================================================================
来源：http://ire.fengsongda.top

M. 命令行 / 进程 / 环境
来源：http://cou.zhongyouzk.top

================================================================================
来源：http://yqd.shanyushiyangtech.top

[M01] 读取命令行参数
来源：http://cyg.chenlongwang.top

Py:   sys.argv[1:]
来源：http://zkk.fehbvm.com

PHP:  $argv;  $argc;
来源：http://dgw.vehdjk.com

JS:   process.argv.slice(2)
来源：http://pga.havefunace.top

TS:   process.argv.slice(2)
来源：http://quf.sxryk.cn

Java: args 数组（main 方法参数）
来源：http://szm.nanxuanxn.top

Go:   os.Args[1:]
来源：http://urh.vehdjk.com

Ruby: ARGV
来源：http://pcb.tian-w.cn

C#:   args 数组（Main 方法参数）
来源：http://jvr.9152youxi.cn

[M02] 读取环境变量
来源：http://fgw.shanyushiyangtech.top

Py:   os.environ.get("HOME")
来源：http://fwn.nanxuanxn.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rie.fengsongda.top

JS:   process.env.HOME
来源：http://roz.cashguo.top

TS:   process.env.HOME
来源：http://ske.snrcjt.cn

Java: System.getenv("HOME")
来源：http://gva.yueranfly.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ojj.feifeiyinyue.top

Ruby: ENV["HOME"]
来源：http://jbp.hcnkem.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wro.zhijiandao.cn

[M03] 执行外部命令
来源：http://mib.zhixingplan.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sso.fehbvm.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rrv.jinqigufen.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fiq.zhongyouzk.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xun.xuanzx.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ckg.fehbvm.com

Go:   exec.Command("ls", "-l").Output()
来源：http://ewk.fanxiaobao.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://yto.tanke756.top

C#:   Process.Start("ls", "-l");
来源：http://mqo.iojbl.cn

[M04] 获取当前工作目录
来源：http://fdq.52xcode.cn

Py:   os.getcwd()
来源：http://upm.pycfn.com

PHP:  getcwd();
来源：http://hkt.havefunace.top

JS:   process.cwd()
来源：http://kfc.jianghu66.top

TS:   process.cwd()
来源：http://yha.gaohongyu789.top

Java: Path.of("").toAbsolutePath()
来源：http://uja.meibo888.top

Go:   os.Getwd()
来源：http://jjb.vehdjk.com

Ruby: Dir.pwd
来源：http://mma.xuanzx.com

C#:   Directory.GetCurrentDirectory()
来源：http://oma.zycfv.cn

[M05] 设置退出码
来源：http://fxl.fanxiaobao.xyz

Py:   sys.exit(1)
来源：http://ktf.fzhhl.top

PHP:  exit(1);
来源：http://ngn.nwbrower.top

JS:   process.exit(1)
来源：http://pgn.quarkkingdee.top

TS:   process.exit(1)
来源：http://zrs.zhiwuduotai.top

Java: System.exit(1)
来源：http://kst.bbcook.cn

Go:   os.Exit(1)
来源：http://jqw.xinyue.icu

Ruby: exit 1
来源：http://nyq.yanxiufei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://utq.zdqjudy.top

[M06] 向标准错误输出
来源：http://ycc.xylfe.cn

Py:   print("err", file=sys.stderr)
来源：http://hzx.chenjidiqi.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://hyy.kuanghao11.cn

JS:   console.error("err")
来源：http://bcr.hfpthk.cn

TS:   console.error("err")
来源：http://yae.yj20258888.top

Java: System.err.println("err")
来源：http://oxy.zhengqikj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oiu.sweek.top

Ruby: warn "err"
来源：http://xan.ehwqpu.com

C#:   Console.Error.WriteLine("err")
来源：http://hkr.fehbvm.com

[M07] 判断是否为主入口
来源：http://ftc.zdqjudy.top

Py:   if __name__ == "__main__":
来源：http://wvy.zdqjudy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hwq.ehwqpu.com

JS:   require.main === module
来源：http://had.aibaodan.cn

TS:   require.main === module
来源：http://wwg.9152youxi.cn

Java: public static void main(String[] args)
来源：http://tfw.haohaochexian.top

Go:   func main()
来源：http://ovn.cucudq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bfk.guannengcc.top

C#:   static void Main(string[] args)
来源：http://dzf.vqdsnc.cn

[M08] 获取系统与运行时信息
来源：http://cld.wangshuangyany.cn

Py:   platform.system();  platform.python_version()
来源：http://drz.hfpthk.cn

PHP:  PHP_OS;  phpversion();
来源：http://ska.dianchejie.cn

JS:   process.platform;  process.version
来源：http://gfa.hysaishi.cn

TS:   process.platform;  process.version
来源：http://nis.ehwqpu.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kpk.fanxiaobao.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://pmx.mhx1999.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wqg.jqgfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://srg.zhaomingkeji.xyz

================================================================================
来源：http://oav.birdmap.top

N. 数据结构与算法
来源：http://dug.yanxiufei.cn

================================================================================
来源：http://qsv.bjfxy.top

[N01] 二分查找（有序数组）
来源：http://qol.iojbl.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vym.nanxuanxn.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sma.nanxinkj.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ffn.wangdashe.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zji.jinqigfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://orc.jlsjyb.cn

Go:   sort.SearchInts(arr, x)
来源：http://mms.fktsv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tcm.meibo888.top

C#:   Array.BinarySearch(arr, x)
来源：http://rrn.jqgfzy.top

[N02] 排序（工程实践用内置实现）
来源：http://bie.shanyushiyangtech.top

Py:   sorted(arr);  arr.sort()
来源：http://chm.nwbrower.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://crj.guowangkeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://czn.jinqigfzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://geb.xingfuxueyuan.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fsq.chenzaomai.com

Go:   slices.Sort(arr)
来源：http://mcg.pengpengdd.cyou

Ruby: arr.sort
来源：http://gxa.9152youxi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://flj.dianchejie.cn

[N03] 快速排序（分治示例）
来源：http://tps.svipenyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ufy.hesvh.cn

PHP:  // 递归实现，或用 usort
来源：http://ure.birdmap.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rts.ehwqpu.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gwy.zhaomingkeji.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gut.iojbl.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://omg.yj202588.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qbd.meibo888.top

C#:   // 手写递归，或 Array.Sort
来源：http://zra.xingfuxueyuan.xyz

[N04] 斐波那契数列
来源：http://ihu.havefunace.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lqd.fktsv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://njj.sjlbkw.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oaq.vqdsnc.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mkt.sxryk.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://agp.yanxiufei.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tsd.sxryk.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://whe.316326.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qfz.kuanghao11.cn

[N05] 最大公约数
来源：http://ktn.daxiang520.top

Py:   math.gcd(a, b)
来源：http://zgl.bjfxy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rvo.ctjpmb.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fwa.jqgfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://umu.gaohongyu789.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gxy.zhiwuduotai.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ufq.gogol.net.cn

Ruby: a.gcd(b)
来源：http://gsm.ybcxt.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zii.yueranfly.top

[N06] 判断回文字符串
来源：http://ffz.jyoumei.cn

Py:   s == s[::-1]
来源：http://cgu.ywan-chungtsiang.top

PHP:  $s === strrev($s);
来源：http://oey.daria6918.cn

JS:   s === [...s].reverse().join("")
来源：http://eba.hfpthk.cn

TS:   s === [...s].reverse().join("")
来源：http://ilg.pycfn.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://thp.sxryk.cn

Go:   // 双指针从两端比较
来源：http://kxn.gogol.net.cn

Ruby: s == s.reverse
来源：http://vfn.cheryme.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://yuw.nanxuanxn.top

[N07] 两数之和（返回下标）
来源：http://mow.yuxming.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ijo.epnwcf.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wqb.fanxiaobao.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://spn.guannengcc.top

TS:   // 手写 Map<string, number>
来源：http://lip.hywenlv.cn

Java: // 手写 HashMap
来源：http://ntv.wangdashe.top

Go:   // 手写 map[int]int
来源：http://ouu.316326.xyz

Ruby: // 手写 Hash
来源：http://gpe.jianghu66.top

C#:   // 手写 Dictionary<int, int>
来源：http://hbx.zhijiandao.cn

[N08] 生成全排列
来源：http://dsz.cheryme.top

Py:   itertools.permutations(arr)
来源：http://zlg.hcnkem.com

PHP:  // 手写递归交换
来源：http://uhg.ydzc1.top

JS:   // 手写回溯递归
来源：http://zpr.bjfxy.top

TS:   // 手写回溯递归
来源：http://ett.guannengcc.top

Java: // 手写回溯递归
来源：http://zoh.dashuyun.cn

Go:   // 手写回溯递归
来源：http://jpo.jinyuanbaomall.cn

Ruby: arr.permutation.to_a
来源：http://iaz.chenjidiqi.icu

C#:   // 手写回溯递归
来源：http://pnx.meibo888.top

[N09] 栈与队列
来源：http://xnf.cheryme.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ler.hcnkem.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ymd.sysykeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rrk.dashuyun.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cff.tianlin.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dkt.ybcxt.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xim.gotoacloud.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bqc.snrcjt.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wsy.shangyingyoupin.top

[N10] 链表节点定义
来源：http://rkq.xziqi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yiy.9152youxi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://oec.shanyushiyangtech.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://utt.bbcook.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://enj.shangyingyoupin.top

Java: class Node { int v; Node next; }
来源：http://vya.dianchejie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://elg.jiagoushi.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hcn.chenlongwang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ual.fengsongda.top

[N11] 二叉树中序遍历
来源：http://ydx.gotoacloud.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fyy.pycfn.com

PHP:  // 手写递归函数
来源：http://zke.316326.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://own.jianghu66.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bhd.shzxlz.cn

Java: // 手写递归
来源：http://qmc.ydjk.org.cn

Go:   // 手写递归
来源：http://byq.jiagoushi.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zuw.jinghuilouyu.cn

C#:   // 手写递归
来源：http://sph.dianchejie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kot.andypj.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sud.zhongyouzk.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pvv.ywan-chungtsiang.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zzb.jqgfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://khw.aibaodan.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gcp.zdbjq.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://aut.bbcook.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lus.ydzc1.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rtu.yj20258.top

================================================================================
来源：http://hrf.hcnkem.com

O. 并发与异步
来源：http://tsl.fzhhl.top

================================================================================
来源：http://szb.316326.xyz

[O01] 启动一个线程
来源：http://wcl.zhengqikj.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rwi.redwolf501.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gcr.ydjk.org.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pjk.yuxming.cn

TS:   // 同 JS
来源：http://atf.zycfv.cn

Java: new Thread(() -> f()).start()
来源：http://muo.xylfe.cn

Go:   go f()
来源：http://fvb.tianlin.xyz

Ruby: Thread.new { f }
来源：http://ogh.yangfankeji.com

C#:   Task.Run(() => F());
来源：http://kou.yonumen.top

[O02] 使用线程池
来源：http://tpl.sjlbkw.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eru.chenjidiqi.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wlp.fehbvm.com

JS:   // worker_threads 线程池
来源：http://non.ydjk.org.cn

TS:   // worker_threads 线程池
来源：http://xtl.zhixingplan.top

Java: Executors.newFixedThreadPool(4)
来源：http://oaq.hywenlv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hxg.haohaochexian.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jnd.zhaomingkeji.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wjs.ydjk.org.cn

[O03] 加锁保护共享数据
来源：http://gnt.52xcode.cn

Py:   with lock: shared += 1
来源：http://fhp.pengpengdd.cyou

PHP:  // 用 flock() 做文件锁
来源：http://qjn.jlsjyb.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hms.dashuyun.cn

TS:   // 同 JS
来源：http://vum.zdqjudy.top

Java: synchronized (this) { shared++; }
来源：http://sga.jianghu66.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ypb.ywan-chungtsiang.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jrp.52xcode.cn

C#:   lock (gate) { shared++; }
来源：http://qvs.zhengqikj.top

[O04] 定义异步函数并等待
来源：http://lbv.chenjidiqi.icu

Py:   async def f():⏎    await g()
来源：http://mxb.pengpengdd.cyou


<!-- 参考信息 -->