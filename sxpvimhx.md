代发 wailian999

[K06] 解析 URL 查询串
来源：http://voc.ehwqpu.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cnn.nanxuanxn.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jmp.gogol.net.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jye.smart0.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sei.hcnkem.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wbg.yonumen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://tdc.xuanzx.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rgr.yj20258.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://azu.xuanzx.com

[K07] 进制转换
来源：http://wdy.zhixingplan.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sfe.sufxvd.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ybo.zhengqikj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lht.ivvv.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qyv.xinyue.icu

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tdo.yj20258.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dsr.0kj1m.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dgm.wangdashe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tyu.birdmap.top

[K08] 二进制序列化（非 JSON）
来源：http://cus.epnwcf.com

Py:   pickle.dumps(obj)
来源：http://kbf.zhixingplan.top

PHP:  serialize($obj);  unserialize($s);
来源：http://sqq.wangshuangyany.cn

JS:   v8.serialize(obj)        // Node
来源：http://poh.bjfxy.top

TS:   v8.serialize(obj)        // Node
来源：http://edp.xingfuxueyuan.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ffr.ywan-chungtsiang.top

Go:   encoding/gob
来源：http://lvv.0kj1m.cn

Ruby: Marshal.dump(obj)
来源：http://vab.c1oappe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ovb.fktsv.cn

================================================================================
来源：http://vgr.sysykeji.top

L. 网络请求
来源：http://wwe.zdqjudy.top

================================================================================
来源：http://snq.52xcode.cn

[L01] 发送 GET 请求
来源：http://qet.jqgufenzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zoc.kuanghao11.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://urq.shangyingyoupin.top

JS:   await fetch(url)
来源：http://ian.xingfuxueyuan.xyz

TS:   await fetch(url)
来源：http://xxr.chenjidiqi.icu

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yic.shangyingyoupin.top

Go:   resp, err := http.Get(url)
来源：http://aaf.yj20258888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://keh.chenjidiqi.icu

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ipl.zdbjq.cn

[L02] 发送 POST JSON
来源：http://oys.yongpay.top

Py:   requests.post(url, json={"a": 1})
来源：http://ycs.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jrq.chenlongwang.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iwu.zhixingplan.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nyw.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pjf.jinqigufen.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wlt.svipenyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hid.aibaodan.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vvs.zhijiandao.cn

[L03] 设置自定义请求头
来源：http://bdu.andypj.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ilu.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://idc.meibo888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://okh.tanke756.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dyr.zhijiandao.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gyk.daxiang520.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://afu.chenlongwang.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wsz.0kj1m.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jzb.zdbjq.cn

[L04] 设置超时
来源：http://acz.ydjk.org.cn

Py:   requests.get(url, timeout=5)
来源：http://kbw.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lwo.jinyuanbaomall.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zdl.sjlbkw.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uhy.yonumen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ibs.feifeiyinyue.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tkn.316326.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ibi.cqqwz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ouu.hesvh.cn

[L05] 上传文件（multipart）
来源：http://moc.nanxuanxn.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jqt.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dao.hfpthk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ipe.ppjwa.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://trf.shuidangran.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qwl.yj202588.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eyq.yueranfly.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ewx.zhoulong.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://elh.hongshengwenyu.top

[L06] 解析响应为 JSON
来源：http://hsy.mhx1999.top

Py:   resp.json()
来源：http://suf.chenlongwang.top

PHP:  json_decode($body, true);
来源：http://qcy.havefunace.top

JS:   await resp.json()
来源：http://esy.jiagoushi.top

TS:   await resp.json()
来源：http://xyy.jinyuanbaomall.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://adh.sysykeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ggx.jinyuanbaomall.cn

Ruby: JSON.parse(resp.body)
来源：http://sjq.52xcode.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://huk.xuanzx.com

[L07] 处理 HTTP 状态码
来源：http://kja.nanxinkj.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mju.gaohongyu789.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lek.yuanzhike.top

JS:   resp.ok;  resp.status
来源：http://qpv.wangdashe.top

TS:   resp.ok;  resp.status
来源：http://bpv.kuanghao11.cn

Java: resp.statusCode()
来源：http://zgf.zdbjq.cn

Go:   resp.StatusCode
来源：http://tpe.shanyushiyangtech.top

Ruby: resp.code.to_i
来源：http://diy.smart0.xyz

C#:   (int)resp.StatusCode
来源：http://dtf.redwolf501.top

[L08] 并发请求多个地址
来源：http://ygw.aibaodan.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zse.yj20258.top

PHP:  curl_multi_init() 系列
来源：http://iyd.zhiwuduotai.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pwr.cqqwz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nsc.yj20258.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ass.jiagoushi.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hdk.nanxuanxn.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qpw.jyoumei.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zen.aizwys.cn

================================================================================
来源：http://day.zhijiandao.cn

M. 命令行 / 进程 / 环境
来源：http://okd.sweek.top

================================================================================
来源：http://ubd.yuxming.cn

[M01] 读取命令行参数
来源：http://oig.sxryk.cn

Py:   sys.argv[1:]
来源：http://tgb.sxryk.cn

PHP:  $argv;  $argc;
来源：http://cem.guannengcc.top

JS:   process.argv.slice(2)
来源：http://fzh.ydjk.org.cn

TS:   process.argv.slice(2)
来源：http://zwv.feifeiyinyue.top

Java: args 数组（main 方法参数）
来源：http://jch.ydjk.org.cn

Go:   os.Args[1:]
来源：http://mrr.sufxvd.cn

Ruby: ARGV
来源：http://kmg.xziqi.cn

C#:   args 数组（Main 方法参数）
来源：http://nkf.shzxlz.cn

[M02] 读取环境变量
来源：http://xbi.vqdsnc.cn

Py:   os.environ.get("HOME")
来源：http://wbp.tarul.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://znm.dashuyun.cn

JS:   process.env.HOME
来源：http://sss.nanxinkj.top

TS:   process.env.HOME
来源：http://iaz.vehdjk.com

Java: System.getenv("HOME")
来源：http://njc.yj20258888.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://onz.sysykeji.top

Ruby: ENV["HOME"]
来源：http://xyg.shuidangran.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xdw.aibaodan.cn

[M03] 执行外部命令
来源：http://kbw.pycfn.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vjt.hfpthk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fnl.snrcjt.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ztq.haohaochexian.top

TS:   child_process.execSync("ls -l").toString()
来源：http://roc.tanke756.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sru.fanxiaobao.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://qch.daxiang520.top

Ruby: system("ls -l");  `ls -l`
来源：http://yxr.c1oappe.top

C#:   Process.Start("ls", "-l");
来源：http://sfl.fzhhl.top

[M04] 获取当前工作目录
来源：http://sbl.ywan-chungtsiang.top

Py:   os.getcwd()
来源：http://oww.chenjidiqi.icu

PHP:  getcwd();
来源：http://spm.aizwys.cn

JS:   process.cwd()
来源：http://jtn.zdqjudy.top

TS:   process.cwd()
来源：http://qas.xingfuxueyuan.xyz

Java: Path.of("").toAbsolutePath()
来源：http://moc.jyoumei.cn

Go:   os.Getwd()
来源：http://kip.kuanghao11.cn

Ruby: Dir.pwd
来源：http://cos.ivvv.top

C#:   Directory.GetCurrentDirectory()
来源：http://vop.feifeiyinyue.top

[M05] 设置退出码
来源：http://dpx.yonumen.top

Py:   sys.exit(1)
来源：http://ckt.zhijiandao.cn

PHP:  exit(1);
来源：http://hfu.sweek.top

JS:   process.exit(1)
来源：http://jce.andypj.xyz

TS:   process.exit(1)
来源：http://plj.bjfxy.top

Java: System.exit(1)
来源：http://gyn.quarkkingdee.top

Go:   os.Exit(1)
来源：http://kne.jiagoushi.top

Ruby: exit 1
来源：http://wjq.feifeiyinyue.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cyl.shanyushiyangkeji.top

[M06] 向标准错误输出
来源：http://cri.jinqigufen.top

Py:   print("err", file=sys.stderr)
来源：http://jyd.jqgufenzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://kfx.bjfxy.top

JS:   console.error("err")
来源：http://uau.jqgufenzy.top

TS:   console.error("err")
来源：http://ory.daxiang520.top

Java: System.err.println("err")
来源：http://xnj.0kj1m.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wrk.epnwcf.com

Ruby: warn "err"
来源：http://ixs.yj202588.top

C#:   Console.Error.WriteLine("err")
来源：http://emb.xinyue.icu

[M07] 判断是否为主入口
来源：http://kwn.yangfankeji.com

Py:   if __name__ == "__main__":
来源：http://edx.nanxuanxn.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xpr.fktsv.cn

JS:   require.main === module
来源：http://ckd.wangdashe.top

TS:   require.main === module
来源：http://jub.sweek.top

Java: public static void main(String[] args)
来源：http://qks.shanyushiyangtech.top

Go:   func main()
来源：http://uuz.hfpthk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://twq.uphjek.com

C#:   static void Main(string[] args)
来源：http://fwc.guannengcc.top

[M08] 获取系统与运行时信息
来源：http://tlv.kuanghao11.cn

Py:   platform.system();  platform.python_version()
来源：http://eum.yueranfly.top

PHP:  PHP_OS;  phpversion();
来源：http://bhn.c1oappe.top

JS:   process.platform;  process.version
来源：http://mqe.xuanzx.com

TS:   process.platform;  process.version
来源：http://zii.smart0.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xcf.xziqi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cho.nwbrower.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zeg.shanyushiyangkeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hdj.wangshuangyany.cn

================================================================================
来源：http://xtf.hnxiangtu.top

N. 数据结构与算法
来源：http://nyu.hysaishi.cn

================================================================================
来源：http://gcw.shzxlz.cn

[N01] 二分查找（有序数组）
来源：http://nko.iojbl.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vwr.guannengcc.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rkn.snrcjt.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cyj.meibo888.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yqj.yuanzhike.top

Java: Arrays.binarySearch(arr, x)
来源：http://oih.fengsongda.top

Go:   sort.SearchInts(arr, x)
来源：http://zbe.yueranfly.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zgz.hongshengwenyu.top

C#:   Array.BinarySearch(arr, x)
来源：http://zlh.zhaomingkeji.xyz

[N02] 排序（工程实践用内置实现）
来源：http://duy.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://zfs.fanxiaobao.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ecq.xylfe.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://oew.ywan-chungtsiang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rok.sweek.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nyp.yonumen.top

Go:   slices.Sort(arr)
来源：http://brj.zhixingplan.top

Ruby: arr.sort
来源：http://fvb.nanxinkj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ehf.shanyushiyangkeji.top

[N03] 快速排序（分治示例）
来源：http://ddx.kuanghao11.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zwk.zhijiandao.cn

PHP:  // 递归实现，或用 usort
来源：http://rbg.zhixingplan.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tst.ivvv.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wkd.shanyushiyangkeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hcl.pengpengdd.cyou

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jze.gogol.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lbz.hnqzz.top

C#:   // 手写递归，或 Array.Sort
来源：http://vkg.bjfxy.top

[N04] 斐波那契数列
来源：http://fpd.jinyuanbaomall.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://knd.xingfuxueyuan.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ymr.andypj.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ogk.gotoacloud.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gom.hnqzz.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pxe.hammf.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qiz.pycfn.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jew.chenjidiqi.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ftl.zhoulong.xyz

[N05] 最大公约数
来源：http://rua.ehwqpu.com

Py:   math.gcd(a, b)
来源：http://djs.fanxiaobao.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://udy.52xcode.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xik.chenzaomai.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lxg.gaohongyu789.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://scj.yueranfly.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ztz.jqgufenzy.top

Ruby: a.gcd(b)
来源：http://esd.nanxuanxn.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mcr.aibaodan.cn

[N06] 判断回文字符串
来源：http://gxc.zhaomingkeji.xyz

Py:   s == s[::-1]
来源：http://xuy.jinghuilouyu.cn

PHP:  $s === strrev($s);
来源：http://ywc.bjfxy.top

JS:   s === [...s].reverse().join("")
来源：http://hxo.meibo888.top

TS:   s === [...s].reverse().join("")
来源：http://koc.vehdjk.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dbq.ybcxt.top

Go:   // 双指针从两端比较
来源：http://zax.smart0.xyz

Ruby: s == s.reverse
来源：http://otl.zhoulong.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://pya.zhengqikj.top

[N07] 两数之和（返回下标）
来源：http://ykm.pycfn.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pbs.cucudq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lnb.meibo888.top

JS:   // 手写 Map：map.set(v, i)
来源：http://fxu.yuxming.cn

TS:   // 手写 Map<string, number>
来源：http://gtc.shanyushiyangkeji.top

Java: // 手写 HashMap
来源：http://loy.hysaishi.cn

Go:   // 手写 map[int]int
来源：http://cgf.hcnkem.com

Ruby: // 手写 Hash
来源：http://pxt.cdnleiting.top

C#:   // 手写 Dictionary<int, int>
来源：http://ddr.shzxlz.cn

[N08] 生成全排列
来源：http://fkb.cdnleiting.top

Py:   itertools.permutations(arr)
来源：http://dlp.fzhhl.top

PHP:  // 手写递归交换
来源：http://gxd.smart0.xyz

JS:   // 手写回溯递归
来源：http://kig.vehdjk.com

TS:   // 手写回溯递归
来源：http://iyr.bbcook.cn

Java: // 手写回溯递归
来源：http://mfq.andypj.xyz

Go:   // 手写回溯递归
来源：http://jzc.yueranfly.top

Ruby: arr.permutation.to_a
来源：http://gpp.hfpthk.cn

C#:   // 手写回溯递归
来源：http://aty.sjlbkw.cn

[N09] 栈与队列
来源：http://phb.xuanzx.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hbf.smart0.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://scg.jlsjyb.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://deo.52xcode.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://abp.jinghuilouyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rox.hfpthk.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://knj.havefunace.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dmp.hongshengwenyu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pyk.yangfankeji.com

[N10] 链表节点定义
来源：http://wke.gogol.net.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://waa.shuidangran.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ush.zhengqikj.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kgc.zdqjudy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qbs.wangdashe.top

Java: class Node { int v; Node next; }
来源：http://otf.wangshuangyany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://oqp.zdqjudy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://gco.ydzc1.top

C#:   class Node { public int V; public Node? Next; }
来源：http://qit.nanxinkj.top

[N11] 二叉树中序遍历
来源：http://dtt.wangdashe.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dyh.tanke756.top

PHP:  // 手写递归函数
来源：http://mod.xylfe.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rcq.vehdjk.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mfc.ctjpmb.com

Java: // 手写递归
来源：http://kzi.yvedp.cn

Go:   // 手写递归
来源：http://hym.fehbvm.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://upn.zhaomingkeji.xyz

C#:   // 手写递归
来源：http://ucy.hfpthk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qct.yuxming.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://btc.xziqi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zfz.ywan-chungtsiang.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dki.guannengcc.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uis.haohaochexian.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hnf.jyoumei.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://egl.ydzc1.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ohb.jiagoushi.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kcp.zhaomingkeji.xyz

================================================================================
来源：http://ddo.zycfv.cn

O. 并发与异步
来源：http://yqc.sysykeji.top

================================================================================
来源：http://fjn.hysaishi.cn

[O01] 启动一个线程
来源：http://fjt.sjlbkw.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yqb.chenjidiqi.icu

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xdw.dianchejie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://khk.hysaishi.cn

TS:   // 同 JS
来源：http://cel.pycfn.com

Java: new Thread(() -> f()).start()
来源：http://vxb.yj20258.top

Go:   go f()
来源：http://xbf.ivvv.top

Ruby: Thread.new { f }
来源：http://tqg.hcnkem.com

C#:   Task.Run(() => F());
来源：http://ckh.xziqi.cn


<!-- 参考信息 -->