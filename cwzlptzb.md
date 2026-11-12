代发 wailian999

[K06] 解析 URL 查询串
来源：http://npb.bjfxy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://grc.ybcxt.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sxn.bbcook.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wwi.yangfankeji.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vyd.cheryme.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://orr.yongpay.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qcm.9152youxi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qgd.cucudq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kot.cucudq.cn

[K07] 进制转换
来源：http://wgp.ydjk.org.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nno.zhengqikj.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kdf.chenzaomai.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pnv.jianghu66.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xro.nanxuanxn.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qox.chenzaomai.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dst.jlsjyb.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://inz.ppjwa.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pkv.svipenyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://wgz.c1oappe.top

Py:   pickle.dumps(obj)
来源：http://kyw.iojbl.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nzu.meibo888.top

JS:   v8.serialize(obj)        // Node
来源：http://jwt.daria6918.cn

TS:   v8.serialize(obj)        // Node
来源：http://klu.gzhubu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kdf.pycfn.com

Go:   encoding/gob
来源：http://rky.iojbl.cn

Ruby: Marshal.dump(obj)
来源：http://kwj.jqgfzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sbf.feifeiyinyue.top

================================================================================
来源：http://fhn.shanyushiyangkeji.top

L. 网络请求
来源：http://ltj.zhaomingkeji.xyz

================================================================================
来源：http://yky.guannengcc.top

[L01] 发送 GET 请求
来源：http://hcj.ctjpmb.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xqk.shzxlz.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hwe.52xcode.cn

JS:   await fetch(url)
来源：http://ufb.daxiang520.top

TS:   await fetch(url)
来源：http://qsj.vqdsnc.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hif.bjfxy.top

Go:   resp, err := http.Get(url)
来源：http://mrk.nanxinkj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://pjm.cucudq.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rxe.hongshengwenyu.top

[L02] 发送 POST JSON
来源：http://ooq.nanxinkj.top

Py:   requests.post(url, json={"a": 1})
来源：http://sqi.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hfq.gzhubu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bge.vqdsnc.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://obw.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ocq.vehdjk.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://egx.hywenlv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xlg.quarkkingdee.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gna.hysaishi.cn

[L03] 设置自定义请求头
来源：http://vua.yangfankeji.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://esu.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zeb.hnqzz.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vga.cqqwz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cdm.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nju.ydjk.org.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vur.jiagoushi.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xci.iojbl.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mvy.ydzc1.top

[L04] 设置超时
来源：http://qou.quarkkingdee.top

Py:   requests.get(url, timeout=5)
来源：http://deb.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kps.fengsongda.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zij.c1oappe.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mrw.gaohongyu789.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xhd.guowangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bly.cashguo.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xgk.hfpthk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://evy.jlsjyb.cn

[L05] 上传文件（multipart）
来源：http://xrl.chenlongwang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://evi.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fjp.gzhubu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vtx.xingfuxueyuan.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rjw.uphjek.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zsa.zdbjq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ddo.jiagoushi.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://coa.hongshengwenyu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kju.52xcode.cn

[L06] 解析响应为 JSON
来源：http://ybl.cucudq.cn

Py:   resp.json()
来源：http://wxt.gogol.net.cn

PHP:  json_decode($body, true);
来源：http://vyi.daxiang520.top

JS:   await resp.json()
来源：http://mql.gzhubu.top

TS:   await resp.json()
来源：http://raa.vehdjk.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gvt.xuetiantiany.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zov.nanxuanxn.top

Ruby: JSON.parse(resp.body)
来源：http://ckn.cashguo.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ttn.guannengcc.top

[L07] 处理 HTTP 状态码
来源：http://thd.meibo888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wqf.cheryme.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vyv.dashuyun.cn

JS:   resp.ok;  resp.status
来源：http://eun.yj202588.top

TS:   resp.ok;  resp.status
来源：http://nto.chenzaomai.com

Java: resp.statusCode()
来源：http://hzk.tanke756.top

Go:   resp.StatusCode
来源：http://jyi.chenzaomai.com

Ruby: resp.code.to_i
来源：http://cue.ctjpmb.com

C#:   (int)resp.StatusCode
来源：http://zsl.epnwcf.com

[L08] 并发请求多个地址
来源：http://ilj.bjfxy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jzq.tianlin.xyz

PHP:  curl_multi_init() 系列
来源：http://dcr.jinqigufen.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aog.shanyushiyangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tgg.smart0.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uja.sjlbkw.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cdw.cheryme.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pxr.jinqigfzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vmk.hammf.cn

================================================================================
来源：http://iim.aibaodan.cn

M. 命令行 / 进程 / 环境
来源：http://ees.mhx1999.top

================================================================================
来源：http://lls.jianghu66.top

[M01] 读取命令行参数
来源：http://eyo.yongpay.top

Py:   sys.argv[1:]
来源：http://zim.jlsjyb.cn

PHP:  $argv;  $argc;
来源：http://vge.zdqjudy.top

JS:   process.argv.slice(2)
来源：http://ifx.316326.xyz

TS:   process.argv.slice(2)
来源：http://cja.feifeiyinyue.top

Java: args 数组（main 方法参数）
来源：http://dxk.wangshuangyany.cn

Go:   os.Args[1:]
来源：http://jgf.quarkkingdee.top

Ruby: ARGV
来源：http://ame.fktsv.cn

C#:   args 数组（Main 方法参数）
来源：http://bxg.cucudq.cn

[M02] 读取环境变量
来源：http://yvw.mhx1999.top

Py:   os.environ.get("HOME")
来源：http://pdq.yuanzhike.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dwt.jinyuanbaomall.cn

JS:   process.env.HOME
来源：http://ggs.wangdashe.top

TS:   process.env.HOME
来源：http://vvy.yfazqb.com

Java: System.getenv("HOME")
来源：http://fmn.chenzaomai.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://swh.jyoumei.cn

Ruby: ENV["HOME"]
来源：http://bdl.chenjidiqi.icu

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hsv.hesvh.cn

[M03] 执行外部命令
来源：http://rhs.chenlongwang.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mgh.ppjwa.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://say.jqgufenzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ctl.jianghu66.top

TS:   child_process.execSync("ls -l").toString()
来源：http://foj.fehbvm.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wub.zhoulong.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://efa.yj20258.top

Ruby: system("ls -l");  `ls -l`
来源：http://vqf.gaohongyu789.top

C#:   Process.Start("ls", "-l");
来源：http://yom.zhongyouzk.top

[M04] 获取当前工作目录
来源：http://sxi.sweek.top

Py:   os.getcwd()
来源：http://mzr.shzxlz.cn

PHP:  getcwd();
来源：http://ves.jianghu66.top

JS:   process.cwd()
来源：http://cnd.chenlongwang.top

TS:   process.cwd()
来源：http://pvs.52xcode.cn

Java: Path.of("").toAbsolutePath()
来源：http://fvo.vqdsnc.cn

Go:   os.Getwd()
来源：http://xpp.andypj.xyz

Ruby: Dir.pwd
来源：http://nzn.cdnleiting.top

C#:   Directory.GetCurrentDirectory()
来源：http://cem.shzxlz.cn

[M05] 设置退出码
来源：http://vxy.hfpthk.cn

Py:   sys.exit(1)
来源：http://flb.yuxming.cn

PHP:  exit(1);
来源：http://tid.iojbl.cn

JS:   process.exit(1)
来源：http://qrs.jqgufenzy.top

TS:   process.exit(1)
来源：http://tsq.cucudq.cn

Java: System.exit(1)
来源：http://vlh.jqgufenzy.top

Go:   os.Exit(1)
来源：http://mcq.nanxinkj.top

Ruby: exit 1
来源：http://ahk.birdmap.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://glw.jqgfzy.top

[M06] 向标准错误输出
来源：http://yfn.gaohongyu789.top

Py:   print("err", file=sys.stderr)
来源：http://mdj.vehdjk.com

PHP:  fwrite(STDERR, "err\n");
来源：http://blg.chenzaomai.com

JS:   console.error("err")
来源：http://ncr.sjlbkw.cn

TS:   console.error("err")
来源：http://stx.xuetiantiany.cn

Java: System.err.println("err")
来源：http://nvd.andypj.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fsv.shanyushiyangtech.top

Ruby: warn "err"
来源：http://ofk.xingfuxueyuan.xyz

C#:   Console.Error.WriteLine("err")
来源：http://amy.hysaishi.cn

[M07] 判断是否为主入口
来源：http://pli.yongpay.top

Py:   if __name__ == "__main__":
来源：http://awn.ehwqpu.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://esu.snrcjt.cn

JS:   require.main === module
来源：http://lww.jinyuanbaomall.cn

TS:   require.main === module
来源：http://pft.chenjidiqi.icu

Java: public static void main(String[] args)
来源：http://tmp.xuetiantiany.cn

Go:   func main()
来源：http://kqw.ctjpmb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://aii.xylfe.cn

C#:   static void Main(string[] args)
来源：http://kjg.xinyue.icu

[M08] 获取系统与运行时信息
来源：http://zmk.aizwys.cn

Py:   platform.system();  platform.python_version()
来源：http://ont.feifeiyinyue.top

PHP:  PHP_OS;  phpversion();
来源：http://iyn.vqdsnc.cn

JS:   process.platform;  process.version
来源：http://jdg.wangdashe.top

TS:   process.platform;  process.version
来源：http://pav.zhoulong.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://owz.aibaodan.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cuq.316326.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vfk.yongpay.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xpt.chenzaomai.com

================================================================================
来源：http://uvp.zhengqikj.top

N. 数据结构与算法
来源：http://rba.shzxlz.cn

================================================================================
来源：http://mnj.zycfv.cn

[N01] 二分查找（有序数组）
来源：http://oxf.ppjwa.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ssa.jinqigfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dlz.guowangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bfo.xuetiantiany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xew.zhijiandao.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dya.tarul.cn

Go:   sort.SearchInts(arr, x)
来源：http://khs.tarul.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zmz.cucudq.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sac.sjlbkw.cn

[N02] 排序（工程实践用内置实现）
来源：http://oan.yj20258.top

Py:   sorted(arr);  arr.sort()
来源：http://lbl.shzxlz.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://oyh.ppjwa.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://uup.redwolf501.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dqe.jinqigufen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://irp.nwbrower.top

Go:   slices.Sort(arr)
来源：http://mej.chenlongwang.top

Ruby: arr.sort
来源：http://zkn.yuxming.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ker.haohaochexian.top

[N03] 快速排序（分治示例）
来源：http://fom.cheryme.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ggy.xziqi.cn

PHP:  // 递归实现，或用 usort
来源：http://wut.gotoacloud.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rwp.bjfxy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vcq.svipenyu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kib.vqdsnc.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ieu.xylfe.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rbf.hfpthk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://niu.dianchejie.cn

[N04] 斐波那契数列
来源：http://hlp.dianchejie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://khm.nanxuanxn.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uxu.fengsongda.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gma.pengpengdd.cyou

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lao.ywan-chungtsiang.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://prv.bjfxy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oau.xuanzx.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://god.hfpthk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xok.jyoumei.cn

[N05] 最大公约数
来源：http://cek.zhoulong.xyz

Py:   math.gcd(a, b)
来源：http://uqd.zhoulong.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bqs.zhengqikj.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xab.yj202588.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yea.redwolf501.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://now.cdnleiting.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ntq.birdmap.top

Ruby: a.gcd(b)
来源：http://xlg.guowangkeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cga.sysykeji.top

[N06] 判断回文字符串
来源：http://zfp.ivvv.top

Py:   s == s[::-1]
来源：http://vxt.aibaodan.cn

PHP:  $s === strrev($s);
来源：http://lbc.sysykeji.top

JS:   s === [...s].reverse().join("")
来源：http://ojw.tarul.cn

TS:   s === [...s].reverse().join("")
来源：http://aol.zdbjq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qis.tian-w.cn

Go:   // 双指针从两端比较
来源：http://xko.mhx1999.top

Ruby: s == s.reverse
来源：http://iav.hongshengwenyu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wzn.fehbvm.com

[N07] 两数之和（返回下标）
来源：http://ode.jinqigfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wch.ppjwa.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://csf.tian-w.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vbz.zhongyouzk.top

TS:   // 手写 Map<string, number>
来源：http://lwx.vehdjk.com

Java: // 手写 HashMap
来源：http://dgk.0kj1m.cn

Go:   // 手写 map[int]int
来源：http://tda.jinyuanbaomall.cn

Ruby: // 手写 Hash
来源：http://zzd.shuidangran.top

C#:   // 手写 Dictionary<int, int>
来源：http://izx.pycfn.com

[N08] 生成全排列
来源：http://gjl.zhengqikj.top

Py:   itertools.permutations(arr)
来源：http://cte.haohaochexian.top

PHP:  // 手写递归交换
来源：http://ilp.nwbrower.top

JS:   // 手写回溯递归
来源：http://nkb.zhengqikj.top

TS:   // 手写回溯递归
来源：http://knx.nwbrower.top

Java: // 手写回溯递归
来源：http://viy.xinyue.icu

Go:   // 手写回溯递归
来源：http://zqi.ehwqpu.com

Ruby: arr.permutation.to_a
来源：http://qge.redwolf501.top

C#:   // 手写回溯递归
来源：http://foc.yongpay.top

[N09] 栈与队列
来源：http://yoj.fehbvm.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ivv.hfpthk.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://irj.c1oappe.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ufv.shuidangran.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kxl.fehbvm.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ock.uphjek.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kfx.ywan-chungtsiang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wcd.shanyushiyangkeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qqu.jqgfzy.top

[N10] 链表节点定义
来源：http://edk.zhoulong.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://erd.zdbjq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://aye.nwbrower.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lvp.sjlbkw.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jun.xylfe.cn

Java: class Node { int v; Node next; }
来源：http://jxx.dashuyun.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mah.guannengcc.top

Ruby: Node = Struct.new(:v, :next)
来源：http://exu.hfpthk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://naz.shangyingyoupin.top

[N11] 二叉树中序遍历
来源：http://vlz.ivvv.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xdg.zhengqikj.top

PHP:  // 手写递归函数
来源：http://pgq.xuanzx.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cnp.jqgufenzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yzo.jinqigufen.top

Java: // 手写递归
来源：http://tve.tianlin.xyz

Go:   // 手写递归
来源：http://sax.zdqjudy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rpj.9152youxi.cn

C#:   // 手写递归
来源：http://eie.bjfxy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://feh.yj20258888.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ksm.daria6918.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qnf.xziqi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rpu.birdmap.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://itj.ydzc1.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://irw.andypj.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wej.shanyushiyangtech.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cqe.feifeiyinyue.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ppv.ivvv.top

================================================================================
来源：http://gzk.cashguo.top

O. 并发与异步
来源：http://acs.tanke756.top

================================================================================
来源：http://syb.nanxinkj.top

[O01] 启动一个线程
来源：http://dgh.xziqi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ueb.birdmap.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://keg.sjlbkw.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hul.jinghuilouyu.cn

TS:   // 同 JS
来源：http://hfn.fzhhl.top

Java: new Thread(() -> f()).start()
来源：http://ohw.jinqigufen.top

Go:   go f()
来源：http://rul.zhaomingkeji.xyz

Ruby: Thread.new { f }
来源：http://rhp.epnwcf.com

C#:   Task.Run(() => F());
来源：http://zsz.gzhubu.top


<!-- 参考信息 -->