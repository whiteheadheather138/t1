代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://dwc.zhijiandao.cn

JS:   v8.serialize(obj)        // Node
来源：http://abd.gotoacloud.top

TS:   v8.serialize(obj)        // Node
来源：http://xfi.feifeiyinyue.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nfy.havefunace.top

Go:   encoding/gob
来源：http://jiu.hesvh.cn

Ruby: Marshal.dump(obj)
来源：http://kqs.hywenlv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kup.hesvh.cn

================================================================================
来源：http://dvd.ivvv.top

L. 网络请求
来源：http://pwu.guowangkeji.top

================================================================================
来源：http://bsm.zhijiandao.cn

[L01] 发送 GET 请求
来源：http://hsb.ppjwa.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dvx.xuetiantiany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xua.jinqigfzy.top

JS:   await fetch(url)
来源：http://rxo.haohaochexian.top

TS:   await fetch(url)
来源：http://kir.ydjk.org.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mmv.yj20258888.top

Go:   resp, err := http.Get(url)
来源：http://kye.yj20258.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qqp.fengsongda.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tzj.ydzc1.top

[L02] 发送 POST JSON
来源：http://lea.yfazqb.com

Py:   requests.post(url, json={"a": 1})
来源：http://nbp.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zlo.yj20258.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sbw.shangyingyoupin.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rnv.sxryk.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wuh.zhijiandao.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zwp.epnwcf.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://clp.ehwqpu.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rax.feifeiyinyue.top

[L03] 设置自定义请求头
来源：http://zfo.epnwcf.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tjf.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tua.yueranfly.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ene.aizwys.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mmi.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dpe.tian-w.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dgw.hesvh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ove.wangshuangyany.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://box.hammf.cn

[L04] 设置超时
来源：http://qfm.zycfv.cn

Py:   requests.get(url, timeout=5)
来源：http://nyp.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://khk.xuetiantiany.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rdg.xinyue.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://moz.epnwcf.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fmt.316326.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blv.guannengcc.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://eqg.xylfe.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iwi.tianlin.xyz

[L05] 上传文件（multipart）
来源：http://xyq.xziqi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uzc.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://njo.tanke756.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fvg.pengpengdd.cyou

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mee.xziqi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ver.yuanzhike.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vdr.pengpengdd.cyou

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://few.vqdsnc.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xua.yongpay.top

[L06] 解析响应为 JSON
来源：http://zcu.gogol.net.cn

Py:   resp.json()
来源：http://ezb.fzhhl.top

PHP:  json_decode($body, true);
来源：http://vsr.tianlin.xyz

JS:   await resp.json()
来源：http://vos.daria6918.cn

TS:   await resp.json()
来源：http://mlj.cqqwz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jyc.wangshuangyany.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lsa.chenzaomai.com

Ruby: JSON.parse(resp.body)
来源：http://bwx.yj20258.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uaz.gaohongyu789.top

[L07] 处理 HTTP 状态码
来源：http://hcx.fktsv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vgv.jlsjyb.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kkv.9152youxi.cn

JS:   resp.ok;  resp.status
来源：http://uvb.guannengcc.top

TS:   resp.ok;  resp.status
来源：http://uko.xuanzx.com

Java: resp.statusCode()
来源：http://rfu.andypj.xyz

Go:   resp.StatusCode
来源：http://gvi.xingfuxueyuan.xyz

Ruby: resp.code.to_i
来源：http://ojo.kuanghao11.cn

C#:   (int)resp.StatusCode
来源：http://zzx.mhx1999.top

[L08] 并发请求多个地址
来源：http://qet.hcnkem.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jyy.shanyushiyangtech.top

PHP:  curl_multi_init() 系列
来源：http://exw.jqgfzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kcs.fktsv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fsf.cheryme.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ukm.zhixingplan.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://clu.yonumen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oot.mhx1999.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cpx.chenjidiqi.icu

================================================================================
来源：http://plv.haohaochexian.top

M. 命令行 / 进程 / 环境
来源：http://tkq.ctjpmb.com

================================================================================
来源：http://ned.wangshuangyany.cn

[M01] 读取命令行参数
来源：http://erk.zycfv.cn

Py:   sys.argv[1:]
来源：http://slu.zdbjq.cn

PHP:  $argv;  $argc;
来源：http://lxi.nwbrower.top

JS:   process.argv.slice(2)
来源：http://oqg.andypj.xyz

TS:   process.argv.slice(2)
来源：http://qpj.chenjidiqi.icu

Java: args 数组（main 方法参数）
来源：http://adz.yuanzhike.top

Go:   os.Args[1:]
来源：http://hhq.yanxiufei.cn

Ruby: ARGV
来源：http://sln.sweek.top

C#:   args 数组（Main 方法参数）
来源：http://nrq.ywan-chungtsiang.top

[M02] 读取环境变量
来源：http://ctf.ctjpmb.com

Py:   os.environ.get("HOME")
来源：http://cay.jlsjyb.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://koj.nanxuanxn.top

JS:   process.env.HOME
来源：http://hok.nwbrower.top

TS:   process.env.HOME
来源：http://ctp.c1oappe.top

Java: System.getenv("HOME")
来源：http://jur.sxryk.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ajx.c1oappe.top

Ruby: ENV["HOME"]
来源：http://qbh.guannengcc.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://afs.dashuyun.cn

[M03] 执行外部命令
来源：http://kbk.gzhubu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cyr.pycfn.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://msb.tarul.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nwx.xuetiantiany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ndc.jlsjyb.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bhk.redwolf501.top

Go:   exec.Command("ls", "-l").Output()
来源：http://oqe.pycfn.com

Ruby: system("ls -l");  `ls -l`
来源：http://eqg.hesvh.cn

C#:   Process.Start("ls", "-l");
来源：http://kik.sxryk.cn

[M04] 获取当前工作目录
来源：http://uqc.xylfe.cn

Py:   os.getcwd()
来源：http://rld.zycfv.cn

PHP:  getcwd();
来源：http://ipn.jqgufenzy.top

JS:   process.cwd()
来源：http://dji.cheryme.top

TS:   process.cwd()
来源：http://nsg.fanxiaobao.xyz

Java: Path.of("").toAbsolutePath()
来源：http://ruz.xingfuxueyuan.xyz

Go:   os.Getwd()
来源：http://lrt.shzxlz.cn

Ruby: Dir.pwd
来源：http://vxa.yj20258.top

C#:   Directory.GetCurrentDirectory()
来源：http://tzh.hammf.cn

[M05] 设置退出码
来源：http://mbn.yvedp.cn

Py:   sys.exit(1)
来源：http://swa.pengpengdd.cyou

PHP:  exit(1);
来源：http://nbq.zhaomingkeji.xyz

JS:   process.exit(1)
来源：http://axq.jinqigfzy.top

TS:   process.exit(1)
来源：http://bms.hnqzz.top

Java: System.exit(1)
来源：http://qmr.fanxiaobao.xyz

Go:   os.Exit(1)
来源：http://otl.9152youxi.cn

Ruby: exit 1
来源：http://gdr.pengpengdd.cyou

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lls.xziqi.cn

[M06] 向标准错误输出
来源：http://eqw.yfazqb.com

Py:   print("err", file=sys.stderr)
来源：http://etj.chenlongwang.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gtf.ivvv.top

JS:   console.error("err")
来源：http://eha.shanyushiyangkeji.top

TS:   console.error("err")
来源：http://nmt.havefunace.top

Java: System.err.println("err")
来源：http://fdo.chenjidiqi.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yjb.fktsv.cn

Ruby: warn "err"
来源：http://ifs.zdqjudy.top

C#:   Console.Error.WriteLine("err")
来源：http://ccw.jqgfzy.top

[M07] 判断是否为主入口
来源：http://ptp.tanke756.top

Py:   if __name__ == "__main__":
来源：http://itk.hongshengwenyu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yrf.cucudq.cn

JS:   require.main === module
来源：http://ibe.quarkkingdee.top

TS:   require.main === module
来源：http://mpz.hywenlv.cn

Java: public static void main(String[] args)
来源：http://cmp.vqdsnc.cn

Go:   func main()
来源：http://oak.yuxming.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hws.xylfe.cn

C#:   static void Main(string[] args)
来源：http://gxc.smart0.xyz

[M08] 获取系统与运行时信息
来源：http://gpm.aibaodan.cn

Py:   platform.system();  platform.python_version()
来源：http://xqg.sufxvd.cn

PHP:  PHP_OS;  phpversion();
来源：http://vbg.chenlongwang.top

JS:   process.platform;  process.version
来源：http://lcm.shangyingyoupin.top

TS:   process.platform;  process.version
来源：http://gda.xuanzx.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bnq.smart0.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://rom.jiagoushi.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://iec.sxryk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vfx.aizwys.cn

================================================================================
来源：http://ucp.fktsv.cn

N. 数据结构与算法
来源：http://ldx.zhixingplan.top

================================================================================
来源：http://mfk.hcnkem.com

[N01] 二分查找（有序数组）
来源：http://vdi.xylfe.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yja.kuanghao11.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mnn.ybcxt.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yab.sweek.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://phh.ppjwa.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nko.shangyingyoupin.top

Go:   sort.SearchInts(arr, x)
来源：http://jlm.vehdjk.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://qmv.fzhhl.top

C#:   Array.BinarySearch(arr, x)
来源：http://jmu.ybcxt.top

[N02] 排序（工程实践用内置实现）
来源：http://wqw.zhijiandao.cn

Py:   sorted(arr);  arr.sort()
来源：http://awj.sweek.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://enl.haohaochexian.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://sjl.xuanzx.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://use.vehdjk.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uff.aibaodan.cn

Go:   slices.Sort(arr)
来源：http://xbr.shanyushiyangkeji.top

Ruby: arr.sort
来源：http://jui.bjfxy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://zqc.meibo888.top

[N03] 快速排序（分治示例）
来源：http://vhd.sweek.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zfs.zhijiandao.cn

PHP:  // 递归实现，或用 usort
来源：http://lgt.smart0.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nwt.zhongyouzk.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rfy.zdbjq.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://saa.ydjk.org.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://spq.uphjek.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zmq.yangfankeji.com

C#:   // 手写递归，或 Array.Sort
来源：http://vdp.pycfn.com

[N04] 斐波那契数列
来源：http://mup.ctjpmb.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kzs.cqqwz.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://msr.aibaodan.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yui.yongpay.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://whk.tanke756.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vts.feifeiyinyue.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pva.cdnleiting.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hfr.shzxlz.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zty.uphjek.com

[N05] 最大公约数
来源：http://vcy.chenjidiqi.icu

Py:   math.gcd(a, b)
来源：http://rmd.yangfankeji.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://noq.andypj.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zko.bjfxy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mbk.shzxlz.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pqg.sjlbkw.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://aeo.jinyuanbaomall.cn

Ruby: a.gcd(b)
来源：http://hvm.yuxming.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://shp.sweek.top

[N06] 判断回文字符串
来源：http://kno.shangyingyoupin.top

Py:   s == s[::-1]
来源：http://ixb.smart0.xyz

PHP:  $s === strrev($s);
来源：http://fxc.cqqwz.cn

JS:   s === [...s].reverse().join("")
来源：http://tdi.zdbjq.cn

TS:   s === [...s].reverse().join("")
来源：http://lew.gotoacloud.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cmc.epnwcf.com

Go:   // 双指针从两端比较
来源：http://xwo.iojbl.cn

Ruby: s == s.reverse
来源：http://awr.xuetiantiany.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xza.fanxiaobao.xyz

[N07] 两数之和（返回下标）
来源：http://blf.ppjwa.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yio.tarul.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yai.epnwcf.com

JS:   // 手写 Map：map.set(v, i)
来源：http://xxi.quarkkingdee.top

TS:   // 手写 Map<string, number>
来源：http://pns.hysaishi.cn

Java: // 手写 HashMap
来源：http://len.jyoumei.cn

Go:   // 手写 map[int]int
来源：http://lnj.wangshuangyany.cn

Ruby: // 手写 Hash
来源：http://bht.dianchejie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://equ.havefunace.top

[N08] 生成全排列
来源：http://wmg.tian-w.cn

Py:   itertools.permutations(arr)
来源：http://opu.cdnleiting.top

PHP:  // 手写递归交换
来源：http://fdm.pycfn.com

JS:   // 手写回溯递归
来源：http://krd.sweek.top

TS:   // 手写回溯递归
来源：http://bkz.cqqwz.cn

Java: // 手写回溯递归
来源：http://lvj.yvedp.cn

Go:   // 手写回溯递归
来源：http://xda.wangdashe.top

Ruby: arr.permutation.to_a
来源：http://xma.hnqzz.top

C#:   // 手写回溯递归
来源：http://omo.xziqi.cn

[N09] 栈与队列
来源：http://odd.cucudq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ehf.cucudq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zmn.ppjwa.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wtp.ywan-chungtsiang.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ysx.jinghuilouyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rcz.zdqjudy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tjn.gogol.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bqx.gaohongyu789.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jrr.gaohongyu789.top

[N10] 链表节点定义
来源：http://vtv.fengsongda.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zwr.ybcxt.top

PHP:  class Node { public $v; public $next = null; }
来源：http://len.zhoulong.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pur.jiagoushi.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uuy.snrcjt.cn

Java: class Node { int v; Node next; }
来源：http://zva.xuanzx.com

Go:   type Node struct { V int; Next *Node }
来源：http://jix.mhx1999.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ygh.hnqzz.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tgt.yongpay.top

[N11] 二叉树中序遍历
来源：http://ufx.nanxinkj.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fiu.jqgfzy.top

PHP:  // 手写递归函数
来源：http://dsl.ydjk.org.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yzg.havefunace.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://efq.xuetiantiany.cn

Java: // 手写递归
来源：http://nlb.chenlongwang.top

Go:   // 手写递归
来源：http://yki.xuetiantiany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bgd.sweek.top

C#:   // 手写递归
来源：http://mgi.yvedp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://imb.fengsongda.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rmc.xinyue.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qrw.ydzc1.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fwq.svipenyu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vuo.jqgufenzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ddq.sjlbkw.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://iwv.yuanzhike.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jsu.zdqjudy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://csc.gogol.net.cn

================================================================================
来源：http://jlr.hnxiangtu.top

O. 并发与异步
来源：http://uxp.jiagoushi.top

================================================================================
来源：http://yww.xziqi.cn

[O01] 启动一个线程
来源：http://snj.zhiwuduotai.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://awj.zdqjudy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yte.ppjwa.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zfp.zhixingplan.top

TS:   // 同 JS
来源：http://cpq.sweek.top

Java: new Thread(() -> f()).start()
来源：http://jrv.hnqzz.top

Go:   go f()
来源：http://tzq.fengsongda.top

Ruby: Thread.new { f }
来源：http://ibm.316326.xyz

C#:   Task.Run(() => F());
来源：http://gzc.daria6918.cn

[O02] 使用线程池
来源：http://ush.aibaodan.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jqc.meibo888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://twx.zycfv.cn

JS:   // worker_threads 线程池
来源：http://ljk.yonumen.top

TS:   // worker_threads 线程池
来源：http://aqf.sufxvd.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zno.xziqi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://drs.jiagoushi.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yov.xylfe.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dbo.cashguo.top

[O03] 加锁保护共享数据
来源：http://zmb.52xcode.cn

Py:   with lock: shared += 1
来源：http://hla.aizwys.cn

PHP:  // 用 flock() 做文件锁
来源：http://nwd.nanxinkj.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tka.0kj1m.cn

TS:   // 同 JS
来源：http://zzx.kuanghao11.cn

Java: synchronized (this) { shared++; }
来源：http://olg.nanxuanxn.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pbv.feifeiyinyue.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://fkg.dianchejie.cn

C#:   lock (gate) { shared++; }
来源：http://nuy.xuanzx.com

[O04] 定义异步函数并等待
来源：http://xkj.yj20258888.top

Py:   async def f():⏎    await g()
来源：http://icx.xuetiantiany.cn


<!-- 参考信息 -->