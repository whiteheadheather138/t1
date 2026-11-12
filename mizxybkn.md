代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lpy.cdnleiting.top

[K07] 进制转换
来源：http://efc.gaohongyu789.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sdl.wangshuangyany.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bvt.jqgfzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rrj.mhx1999.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vkz.hesvh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tyv.mhx1999.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://eje.nanxuanxn.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nke.xuanzx.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bcj.shzxlz.cn

[K08] 二进制序列化（非 JSON）
来源：http://pgc.ywan-chungtsiang.top

Py:   pickle.dumps(obj)
来源：http://ken.xziqi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://voq.birdmap.top

JS:   v8.serialize(obj)        // Node
来源：http://eki.sjlbkw.cn

TS:   v8.serialize(obj)        // Node
来源：http://mou.pengpengdd.cyou

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bos.zdbjq.cn

Go:   encoding/gob
来源：http://rna.gotoacloud.top

Ruby: Marshal.dump(obj)
来源：http://trm.jlsjyb.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fxn.chenzaomai.com

================================================================================
来源：http://fry.gaohongyu789.top

L. 网络请求
来源：http://wmq.jinghuilouyu.cn

================================================================================
来源：http://dhp.shanyushiyangtech.top

[L01] 发送 GET 请求
来源：http://fha.jinyuanbaomall.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rcc.52xcode.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://eef.vqdsnc.cn

JS:   await fetch(url)
来源：http://irz.nanxinkj.top

TS:   await fetch(url)
来源：http://ryj.bjfxy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://iey.tarul.cn

Go:   resp, err := http.Get(url)
来源：http://egh.xziqi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ekz.yvedp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cls.52xcode.cn

[L02] 发送 POST JSON
来源：http://suo.zhengqikj.top

Py:   requests.post(url, json={"a": 1})
来源：http://rer.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mrs.quarkkingdee.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://odp.jinghuilouyu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bsi.jqgufenzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xhh.quarkkingdee.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://agg.yj202588.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blx.xylfe.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bax.shangyingyoupin.top

[L03] 设置自定义请求头
来源：http://ufg.jinqigfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zhd.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ssx.cheryme.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vok.zdbjq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nuc.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://iyr.uphjek.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://idw.jinyuanbaomall.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lsv.ydjk.org.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pnu.ehwqpu.com

[L04] 设置超时
来源：http://gni.hcnkem.com

Py:   requests.get(url, timeout=5)
来源：http://dvc.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yyn.yueranfly.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jpk.quarkkingdee.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://glk.shuidangran.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rkf.sjlbkw.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://puu.jqgfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mfm.nwbrower.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rjn.sweek.top

[L05] 上传文件（multipart）
来源：http://vyh.zhoulong.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gyv.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ntm.bbcook.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://njz.jinghuilouyu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sbs.tian-w.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hck.yvedp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dga.gogol.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dcp.hesvh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uta.sjlbkw.cn

[L06] 解析响应为 JSON
来源：http://ofm.cucudq.cn

Py:   resp.json()
来源：http://hdy.tian-w.cn

PHP:  json_decode($body, true);
来源：http://pqe.tanke756.top

JS:   await resp.json()
来源：http://bfo.jianghu66.top

TS:   await resp.json()
来源：http://qop.jinyuanbaomall.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://odr.tanke756.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dqo.vehdjk.com

Ruby: JSON.parse(resp.body)
来源：http://esf.andypj.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mkw.fktsv.cn

[L07] 处理 HTTP 状态码
来源：http://lnd.pycfn.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rgn.yanxiufei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nhc.nanxinkj.top

JS:   resp.ok;  resp.status
来源：http://kxl.epnwcf.com

TS:   resp.ok;  resp.status
来源：http://jxs.meibo888.top

Java: resp.statusCode()
来源：http://dky.xuanzx.com

Go:   resp.StatusCode
来源：http://lcc.hnqzz.top

Ruby: resp.code.to_i
来源：http://vld.c1oappe.top

C#:   (int)resp.StatusCode
来源：http://mux.ybcxt.top

[L08] 并发请求多个地址
来源：http://hug.jinghuilouyu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pbn.hysaishi.cn

PHP:  curl_multi_init() 系列
来源：http://xgm.wangshuangyany.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wpa.pengpengdd.cyou

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mrn.cashguo.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://abh.gogol.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hqm.gzhubu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://veo.gaohongyu789.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zmx.iojbl.cn

================================================================================
来源：http://vag.zhijiandao.cn

M. 命令行 / 进程 / 环境
来源：http://zob.hcnkem.com

================================================================================
来源：http://zac.dashuyun.cn

[M01] 读取命令行参数
来源：http://ert.316326.xyz

Py:   sys.argv[1:]
来源：http://qrt.fzhhl.top

PHP:  $argv;  $argc;
来源：http://mex.sweek.top

JS:   process.argv.slice(2)
来源：http://crg.chenzaomai.com

TS:   process.argv.slice(2)
来源：http://asm.hongshengwenyu.top

Java: args 数组（main 方法参数）
来源：http://gsk.jinqigfzy.top

Go:   os.Args[1:]
来源：http://cnd.pengpengdd.cyou

Ruby: ARGV
来源：http://byi.hysaishi.cn

C#:   args 数组（Main 方法参数）
来源：http://dvl.sjlbkw.cn

[M02] 读取环境变量
来源：http://iks.zhiwuduotai.top

Py:   os.environ.get("HOME")
来源：http://hew.tianlin.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wbr.0kj1m.cn

JS:   process.env.HOME
来源：http://boh.kuanghao11.cn

TS:   process.env.HOME
来源：http://tiz.pengpengdd.cyou

Java: System.getenv("HOME")
来源：http://vlb.tarul.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oel.sufxvd.cn

Ruby: ENV["HOME"]
来源：http://ckk.chenzaomai.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cjd.9152youxi.cn

[M03] 执行外部命令
来源：http://wuy.316326.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cxv.fengsongda.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://iik.gotoacloud.top

JS:   child_process.execSync("ls -l").toString()
来源：http://wvx.pengpengdd.cyou

TS:   child_process.execSync("ls -l").toString()
来源：http://all.hcnkem.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ffm.zdbjq.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ewg.zhengqikj.top

Ruby: system("ls -l");  `ls -l`
来源：http://fnh.xinyue.icu

C#:   Process.Start("ls", "-l");
来源：http://wes.jinghuilouyu.cn

[M04] 获取当前工作目录
来源：http://vis.jinghuilouyu.cn

Py:   os.getcwd()
来源：http://qwm.gzhubu.top

PHP:  getcwd();
来源：http://rcb.zhixingplan.top

JS:   process.cwd()
来源：http://ofd.xziqi.cn

TS:   process.cwd()
来源：http://eph.yongpay.top

Java: Path.of("").toAbsolutePath()
来源：http://ejc.fehbvm.com

Go:   os.Getwd()
来源：http://ghk.hnxiangtu.top

Ruby: Dir.pwd
来源：http://doh.shangyingyoupin.top

C#:   Directory.GetCurrentDirectory()
来源：http://gvn.andypj.xyz

[M05] 设置退出码
来源：http://vxl.chenlongwang.top

Py:   sys.exit(1)
来源：http://lel.andypj.xyz

PHP:  exit(1);
来源：http://wnp.hfpthk.cn

JS:   process.exit(1)
来源：http://qpp.gogol.net.cn

TS:   process.exit(1)
来源：http://ujn.tanke756.top

Java: System.exit(1)
来源：http://dva.yonumen.top

Go:   os.Exit(1)
来源：http://xgo.tanke756.top

Ruby: exit 1
来源：http://yte.feifeiyinyue.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xja.hysaishi.cn

[M06] 向标准错误输出
来源：http://ohx.jianghu66.top

Py:   print("err", file=sys.stderr)
来源：http://iec.9152youxi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vof.fehbvm.com

JS:   console.error("err")
来源：http://yfk.yonumen.top

TS:   console.error("err")
来源：http://rom.ywan-chungtsiang.top

Java: System.err.println("err")
来源：http://xmy.9152youxi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ioe.cqqwz.cn

Ruby: warn "err"
来源：http://jbx.ppjwa.cn

C#:   Console.Error.WriteLine("err")
来源：http://jyf.yangfankeji.com

[M07] 判断是否为主入口
来源：http://ylz.yongpay.top

Py:   if __name__ == "__main__":
来源：http://vmx.tian-w.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cos.zhengqikj.top

JS:   require.main === module
来源：http://tzi.haohaochexian.top

TS:   require.main === module
来源：http://qhr.shzxlz.cn

Java: public static void main(String[] args)
来源：http://xra.yuxming.cn

Go:   func main()
来源：http://dbh.hcnkem.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fib.ctjpmb.com

C#:   static void Main(string[] args)
来源：http://uax.jianghu66.top

[M08] 获取系统与运行时信息
来源：http://yfc.hongshengwenyu.top

Py:   platform.system();  platform.python_version()
来源：http://msc.jqgfzy.top

PHP:  PHP_OS;  phpversion();
来源：http://hob.haohaochexian.top

JS:   process.platform;  process.version
来源：http://kvf.tanke756.top

TS:   process.platform;  process.version
来源：http://jur.xuanzx.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gfx.sjlbkw.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qbv.hammf.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hwu.wangshuangyany.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cxt.wangdashe.top

================================================================================
来源：http://txv.hongshengwenyu.top

N. 数据结构与算法
来源：http://jyr.tian-w.cn

================================================================================
来源：http://iuw.hammf.cn

[N01] 二分查找（有序数组）
来源：http://zrc.fktsv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hzv.epnwcf.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mar.birdmap.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bpp.nanxuanxn.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ddt.pycfn.com

Java: Arrays.binarySearch(arr, x)
来源：http://bxb.redwolf501.top

Go:   sort.SearchInts(arr, x)
来源：http://muh.redwolf501.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://pgg.snrcjt.cn

C#:   Array.BinarySearch(arr, x)
来源：http://swc.zhongyouzk.top

[N02] 排序（工程实践用内置实现）
来源：http://nmx.meibo888.top

Py:   sorted(arr);  arr.sort()
来源：http://cvp.shanyushiyangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bjg.fengsongda.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://tty.9152youxi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rbb.dashuyun.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://now.guannengcc.top

Go:   slices.Sort(arr)
来源：http://ztv.aizwys.cn

Ruby: arr.sort
来源：http://vgq.uphjek.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://nmn.guowangkeji.top

[N03] 快速排序（分治示例）
来源：http://lql.fengsongda.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ica.9152youxi.cn

PHP:  // 递归实现，或用 usort
来源：http://pqq.yj20258888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sxd.jinqigfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zed.nwbrower.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xtk.ywan-chungtsiang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://epi.vehdjk.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tfk.sweek.top

C#:   // 手写递归，或 Array.Sort
来源：http://szt.sufxvd.cn

[N04] 斐波那契数列
来源：http://zid.yuanzhike.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wtm.ehwqpu.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mpk.ctjpmb.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ctw.jqgfzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mpb.redwolf501.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rjj.shanyushiyangkeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://frj.xylfe.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xib.zhoulong.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gjb.jiagoushi.top

[N05] 最大公约数
来源：http://uog.xuetiantiany.cn

Py:   math.gcd(a, b)
来源：http://bsx.svipenyu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vxt.yueranfly.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tlm.wangshuangyany.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rlw.xuetiantiany.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uhw.hongshengwenyu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qdb.shzxlz.cn

Ruby: a.gcd(b)
来源：http://bci.feifeiyinyue.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ehe.yueranfly.top

[N06] 判断回文字符串
来源：http://tru.smart0.xyz

Py:   s == s[::-1]
来源：http://izb.sxryk.cn

PHP:  $s === strrev($s);
来源：http://yyl.dashuyun.cn

JS:   s === [...s].reverse().join("")
来源：http://osy.zhaomingkeji.xyz

TS:   s === [...s].reverse().join("")
来源：http://hsw.daxiang520.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pjd.wangdashe.top

Go:   // 双指针从两端比较
来源：http://bmv.shanyushiyangtech.top

Ruby: s == s.reverse
来源：http://ctz.jinqigufen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ckr.birdmap.top

[N07] 两数之和（返回下标）
来源：http://wpx.ybcxt.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://aru.zhongyouzk.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wxd.dianchejie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://plc.sjlbkw.cn

TS:   // 手写 Map<string, number>
来源：http://htu.xinyue.icu

Java: // 手写 HashMap
来源：http://zzn.hesvh.cn

Go:   // 手写 map[int]int
来源：http://pwv.jqgufenzy.top

Ruby: // 手写 Hash
来源：http://lid.hesvh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gzi.sufxvd.cn

[N08] 生成全排列
来源：http://vze.yuxming.cn

Py:   itertools.permutations(arr)
来源：http://dta.fengsongda.top

PHP:  // 手写递归交换
来源：http://nds.uphjek.com

JS:   // 手写回溯递归
来源：http://qmj.316326.xyz

TS:   // 手写回溯递归
来源：http://dep.yonumen.top

Java: // 手写回溯递归
来源：http://yiv.dashuyun.cn

Go:   // 手写回溯递归
来源：http://tkv.ppjwa.cn

Ruby: arr.permutation.to_a
来源：http://bdy.yvedp.cn

C#:   // 手写回溯递归
来源：http://vhw.yj20258888.top

[N09] 栈与队列
来源：http://skh.sysykeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hfp.xingfuxueyuan.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ncf.dashuyun.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://buf.sweek.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cnp.epnwcf.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lxh.zycfv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zzo.jinqigfzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mdu.kuanghao11.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cli.ydjk.org.cn

[N10] 链表节点定义
来源：http://ary.jinghuilouyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://abz.hywenlv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pzi.jlsjyb.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vmo.chenjidiqi.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://aio.52xcode.cn

Java: class Node { int v; Node next; }
来源：http://rly.sjlbkw.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jrg.snrcjt.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gaz.jlsjyb.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zcu.sweek.top

[N11] 二叉树中序遍历
来源：http://fyn.xylfe.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://aea.dianchejie.cn

PHP:  // 手写递归函数
来源：http://vdy.yvedp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lzm.yfazqb.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rsh.yongpay.top

Java: // 手写递归
来源：http://ena.snrcjt.cn

Go:   // 手写递归
来源：http://qdz.uphjek.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vuv.yj20258.top

C#:   // 手写递归
来源：http://fap.snrcjt.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jma.svipenyu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fgv.haohaochexian.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pxf.hammf.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pjd.zhongyouzk.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gcc.c1oappe.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ifs.uphjek.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://csm.ivvv.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tpx.shzxlz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tfv.hesvh.cn

================================================================================
来源：http://uqw.xuanzx.com

O. 并发与异步
来源：http://wxm.fzhhl.top

================================================================================
来源：http://lph.xinyue.icu

[O01] 启动一个线程
来源：http://wyh.bbcook.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ozv.hywenlv.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wfc.316326.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ego.zhoulong.xyz

TS:   // 同 JS
来源：http://axy.yangfankeji.com

Java: new Thread(() -> f()).start()
来源：http://ceh.havefunace.top

Go:   go f()
来源：http://era.epnwcf.com

Ruby: Thread.new { f }
来源：http://czg.ehwqpu.com

C#:   Task.Run(() => F());
来源：http://rph.guowangkeji.top

[O02] 使用线程池
来源：http://twn.vqdsnc.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pad.kuanghao11.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bjx.ppjwa.cn

JS:   // worker_threads 线程池
来源：http://bfg.yongpay.top

TS:   // worker_threads 线程池
来源：http://qcx.meibo888.top

Java: Executors.newFixedThreadPool(4)
来源：http://wwh.sufxvd.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nmq.9152youxi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://znl.pycfn.com


<!-- 参考信息 -->