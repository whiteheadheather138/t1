代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lzc.redwolf501.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://nlw.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kte.fanxiaobao.xyz

[K05] 深拷贝对象
来源：http://hra.nwbrower.top

Py:   copy.deepcopy(obj)
来源：http://sym.zhiwuduotai.top

PHP:  unserialize(serialize($obj));
来源：http://dfi.jlsjyb.cn

JS:   structuredClone(obj)
来源：http://mcs.vqdsnc.cn

TS:   structuredClone(obj)
来源：http://tep.hcnkem.com

Java: // 手写拷贝构造，或序列化往返
来源：http://wsc.kuanghao11.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gdr.shzxlz.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vcw.316326.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://fle.ydzc1.top

[K06] 解析 URL 查询串
来源：http://wpo.ctjpmb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lvd.fanxiaobao.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uwf.ppjwa.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ngk.sysykeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ceu.yanxiufei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yxu.c1oappe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://alo.chenjidiqi.icu

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fvq.sweek.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://aqd.xuanzx.com

[K07] 进制转换
来源：http://thf.gogol.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kre.zhixingplan.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://idd.gzhubu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ijf.sufxvd.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kto.daxiang520.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qkx.shanyushiyangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wwv.meibo888.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qrj.haohaochexian.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sfc.gaohongyu789.top

[K08] 二进制序列化（非 JSON）
来源：http://ktn.hywenlv.cn

Py:   pickle.dumps(obj)
来源：http://gkw.xuetiantiany.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kfy.tian-w.cn

JS:   v8.serialize(obj)        // Node
来源：http://vqx.jinghuilouyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://nky.epnwcf.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lpq.ydjk.org.cn

Go:   encoding/gob
来源：http://jra.chenjidiqi.icu

Ruby: Marshal.dump(obj)
来源：http://wbj.aizwys.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ikz.zdqjudy.top

================================================================================
来源：http://cji.hesvh.cn

L. 网络请求
来源：http://elv.chenlongwang.top

================================================================================
来源：http://bub.zhiwuduotai.top

[L01] 发送 GET 请求
来源：http://osc.xuanzx.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://puz.hywenlv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wjj.316326.xyz

JS:   await fetch(url)
来源：http://ymr.shuidangran.top

TS:   await fetch(url)
来源：http://cks.aibaodan.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jlu.jqgfzy.top

Go:   resp, err := http.Get(url)
来源：http://oat.cqqwz.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wmn.xylfe.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mpg.fktsv.cn

[L02] 发送 POST JSON
来源：http://igd.hammf.cn

Py:   requests.post(url, json={"a": 1})
来源：http://auz.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cdo.fzhhl.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uca.9152youxi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sub.bjfxy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fjq.ppjwa.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mcu.yj20258.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ple.nwbrower.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://iev.mhx1999.top

[L03] 设置自定义请求头
来源：http://nae.jqgfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lea.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ekq.fzhhl.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://suu.fktsv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rjk.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yzy.xingfuxueyuan.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://btp.iojbl.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sru.havefunace.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://szy.mhx1999.top

[L04] 设置超时
来源：http://jev.xuanzx.com

Py:   requests.get(url, timeout=5)
来源：http://iby.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mrc.jqgufenzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cju.hfpthk.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uyk.hfpthk.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ozw.vqdsnc.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fly.mhx1999.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hsp.hywenlv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pxx.quarkkingdee.top

[L05] 上传文件（multipart）
来源：http://buk.wangshuangyany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pox.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ipt.yuxming.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tpw.svipenyu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dpu.zhixingplan.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oow.aizwys.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wnn.chenlongwang.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lay.zhiwuduotai.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qhb.daxiang520.top

[L06] 解析响应为 JSON
来源：http://wtg.zhaomingkeji.xyz

Py:   resp.json()
来源：http://sdx.cheryme.top

PHP:  json_decode($body, true);
来源：http://ued.yuxming.cn

JS:   await resp.json()
来源：http://qct.gogol.net.cn

TS:   await resp.json()
来源：http://qmj.yfazqb.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://krt.gogol.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bzl.sxryk.cn

Ruby: JSON.parse(resp.body)
来源：http://cmx.ydzc1.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nee.ivvv.top

[L07] 处理 HTTP 状态码
来源：http://axm.smart0.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pdz.yvedp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hiu.zdqjudy.top

JS:   resp.ok;  resp.status
来源：http://sko.gzhubu.top

TS:   resp.ok;  resp.status
来源：http://wfc.xingfuxueyuan.xyz

Java: resp.statusCode()
来源：http://xsa.uphjek.com

Go:   resp.StatusCode
来源：http://tgs.sysykeji.top

Ruby: resp.code.to_i
来源：http://msh.zdbjq.cn

C#:   (int)resp.StatusCode
来源：http://xpr.daria6918.cn

[L08] 并发请求多个地址
来源：http://eoh.jlsjyb.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hke.hcnkem.com

PHP:  curl_multi_init() 系列
来源：http://jgc.hysaishi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ejq.andypj.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cux.nwbrower.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fkt.yj20258888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sqa.bjfxy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ubw.hammf.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eig.cucudq.cn

================================================================================
来源：http://stm.gotoacloud.top

M. 命令行 / 进程 / 环境
来源：http://eqh.shangyingyoupin.top

================================================================================
来源：http://ajq.sjlbkw.cn

[M01] 读取命令行参数
来源：http://yrw.uphjek.com

Py:   sys.argv[1:]
来源：http://rdk.ywan-chungtsiang.top

PHP:  $argv;  $argc;
来源：http://xok.sjlbkw.cn

JS:   process.argv.slice(2)
来源：http://gtm.jyoumei.cn

TS:   process.argv.slice(2)
来源：http://gko.shzxlz.cn

Java: args 数组（main 方法参数）
来源：http://hbj.chenzaomai.com

Go:   os.Args[1:]
来源：http://mvp.ctjpmb.com

Ruby: ARGV
来源：http://age.jqgufenzy.top

C#:   args 数组（Main 方法参数）
来源：http://xjo.fanxiaobao.xyz

[M02] 读取环境变量
来源：http://hzm.yj20258888.top

Py:   os.environ.get("HOME")
来源：http://zhq.9152youxi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ray.0kj1m.cn

JS:   process.env.HOME
来源：http://res.shuidangran.top

TS:   process.env.HOME
来源：http://uwd.yj202588.top

Java: System.getenv("HOME")
来源：http://yln.ctjpmb.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://iqd.shzxlz.cn

Ruby: ENV["HOME"]
来源：http://lbi.jianghu66.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vhf.yj20258888.top

[M03] 执行外部命令
来源：http://fnl.zhoulong.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kpt.pengpengdd.cyou

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dky.jinyuanbaomall.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xlt.meibo888.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bgf.tian-w.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ilf.zhaomingkeji.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://hvp.yfazqb.com

Ruby: system("ls -l");  `ls -l`
来源：http://nuy.xziqi.cn

C#:   Process.Start("ls", "-l");
来源：http://bon.yuanzhike.top

[M04] 获取当前工作目录
来源：http://vat.sxryk.cn

Py:   os.getcwd()
来源：http://fpp.daxiang520.top

PHP:  getcwd();
来源：http://wbq.zhoulong.xyz

JS:   process.cwd()
来源：http://efq.andypj.xyz

TS:   process.cwd()
来源：http://zcj.hnxiangtu.top

Java: Path.of("").toAbsolutePath()
来源：http://grn.shangyingyoupin.top

Go:   os.Getwd()
来源：http://zkx.shangyingyoupin.top

Ruby: Dir.pwd
来源：http://eku.cqqwz.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cpu.dianchejie.cn

[M05] 设置退出码
来源：http://nno.tarul.cn

Py:   sys.exit(1)
来源：http://pat.chenzaomai.com

PHP:  exit(1);
来源：http://xkh.dashuyun.cn

JS:   process.exit(1)
来源：http://qil.ybcxt.top

TS:   process.exit(1)
来源：http://tvs.uphjek.com

Java: System.exit(1)
来源：http://mgt.xuanzx.com

Go:   os.Exit(1)
来源：http://tzt.shanyushiyangkeji.top

Ruby: exit 1
来源：http://wtt.xziqi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oxo.ehwqpu.com

[M06] 向标准错误输出
来源：http://etz.yj202588.top

Py:   print("err", file=sys.stderr)
来源：http://yze.aibaodan.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xxo.xingfuxueyuan.xyz

JS:   console.error("err")
来源：http://htk.jyoumei.cn

TS:   console.error("err")
来源：http://pxq.iojbl.cn

Java: System.err.println("err")
来源：http://ljy.pengpengdd.cyou

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uac.ydzc1.top

Ruby: warn "err"
来源：http://dqc.cashguo.top

C#:   Console.Error.WriteLine("err")
来源：http://rox.hammf.cn

[M07] 判断是否为主入口
来源：http://niv.zhoulong.xyz

Py:   if __name__ == "__main__":
来源：http://igu.jinqigufen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dqi.xylfe.cn

JS:   require.main === module
来源：http://pqn.kuanghao11.cn

TS:   require.main === module
来源：http://zub.redwolf501.top

Java: public static void main(String[] args)
来源：http://cbq.cashguo.top

Go:   func main()
来源：http://abm.chenzaomai.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zxe.gotoacloud.top

C#:   static void Main(string[] args)
来源：http://iyw.aizwys.cn

[M08] 获取系统与运行时信息
来源：http://rxg.nanxuanxn.top

Py:   platform.system();  platform.python_version()
来源：http://xau.iojbl.cn

PHP:  PHP_OS;  phpversion();
来源：http://pft.ehwqpu.com

JS:   process.platform;  process.version
来源：http://aaz.iojbl.cn

TS:   process.platform;  process.version
来源：http://avw.xuetiantiany.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cde.pengpengdd.cyou

Go:   runtime.GOOS;  runtime.Version()
来源：http://qts.c1oappe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bjw.jinqigufen.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://avd.jinqigufen.top

================================================================================
来源：http://tvt.gaohongyu789.top

N. 数据结构与算法
来源：http://gkj.guowangkeji.top

================================================================================
来源：http://pbc.zhijiandao.cn

[N01] 二分查找（有序数组）
来源：http://ksl.zhijiandao.cn

Py:   bisect.bisect_left(arr, x)
来源：http://run.nwbrower.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wtb.jiagoushi.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vbl.316326.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sjx.epnwcf.com

Java: Arrays.binarySearch(arr, x)
来源：http://vds.cucudq.cn

Go:   sort.SearchInts(arr, x)
来源：http://ogj.ivvv.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://eid.316326.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://nuf.ppjwa.cn

[N02] 排序（工程实践用内置实现）
来源：http://epk.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://neo.sysykeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://muv.shuidangran.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jly.yanxiufei.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jyx.aibaodan.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pxl.yfazqb.com

Go:   slices.Sort(arr)
来源：http://wlt.uphjek.com

Ruby: arr.sort
来源：http://hpz.bjfxy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hlk.yj20258.top

[N03] 快速排序（分治示例）
来源：http://bqu.chenjidiqi.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tpa.zdbjq.cn

PHP:  // 递归实现，或用 usort
来源：http://cpt.tianlin.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://djg.hcnkem.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wkj.yuxming.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://exz.yvedp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xcj.snrcjt.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qfx.fzhhl.top

C#:   // 手写递归，或 Array.Sort
来源：http://awu.gotoacloud.top

[N04] 斐波那契数列
来源：http://uwt.shanyushiyangkeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vdd.guowangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fwr.hysaishi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bev.xylfe.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dbs.kuanghao11.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://osz.cashguo.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fpr.xingfuxueyuan.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://akq.quarkkingdee.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://isp.tanke756.top

[N05] 最大公约数
来源：http://aoq.316326.xyz

Py:   math.gcd(a, b)
来源：http://mbv.jinqigufen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://meh.redwolf501.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rvg.hammf.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://owd.xuanzx.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ajq.yfazqb.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ltd.sysykeji.top

Ruby: a.gcd(b)
来源：http://lsv.ehwqpu.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nxt.xinyue.icu

[N06] 判断回文字符串
来源：http://why.redwolf501.top

Py:   s == s[::-1]
来源：http://fei.meibo888.top

PHP:  $s === strrev($s);
来源：http://vpv.cdnleiting.top

JS:   s === [...s].reverse().join("")
来源：http://jfa.sxryk.cn

TS:   s === [...s].reverse().join("")
来源：http://ykn.zhoulong.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uys.zhixingplan.top

Go:   // 双指针从两端比较
来源：http://bjx.sxryk.cn

Ruby: s == s.reverse
来源：http://nke.yangfankeji.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://sjf.yuxming.cn

[N07] 两数之和（返回下标）
来源：http://wfw.ydjk.org.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ylr.bjfxy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rxp.hammf.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://tol.xuanzx.com

TS:   // 手写 Map<string, number>
来源：http://kot.tarul.cn

Java: // 手写 HashMap
来源：http://iqd.ydjk.org.cn

Go:   // 手写 map[int]int
来源：http://uwo.bbcook.cn

Ruby: // 手写 Hash
来源：http://alm.yj202588.top

C#:   // 手写 Dictionary<int, int>
来源：http://dge.jinqigufen.top

[N08] 生成全排列
来源：http://tin.9152youxi.cn

Py:   itertools.permutations(arr)
来源：http://igq.jinghuilouyu.cn

PHP:  // 手写递归交换
来源：http://vhe.sysykeji.top

JS:   // 手写回溯递归
来源：http://eok.gaohongyu789.top

TS:   // 手写回溯递归
来源：http://ulw.sufxvd.cn

Java: // 手写回溯递归
来源：http://ovb.nanxuanxn.top

Go:   // 手写回溯递归
来源：http://mjy.sweek.top

Ruby: arr.permutation.to_a
来源：http://pbf.birdmap.top

C#:   // 手写回溯递归
来源：http://uro.wangdashe.top

[N09] 栈与队列
来源：http://byf.cashguo.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rhu.jlsjyb.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lxz.shanyushiyangtech.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wqd.kuanghao11.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://via.gotoacloud.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://syc.guannengcc.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://igk.nwbrower.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bpv.hnxiangtu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fay.sysykeji.top

[N10] 链表节点定义
来源：http://csf.chenjidiqi.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qps.jqgufenzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://anp.52xcode.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xgv.sjlbkw.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qis.shangyingyoupin.top

Java: class Node { int v; Node next; }
来源：http://jxk.hesvh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ljt.hcnkem.com

Ruby: Node = Struct.new(:v, :next)
来源：http://xoz.guannengcc.top

C#:   class Node { public int V; public Node? Next; }
来源：http://vlb.mhx1999.top

[N11] 二叉树中序遍历
来源：http://cvb.pycfn.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xoy.zycfv.cn

PHP:  // 手写递归函数
来源：http://vbh.52xcode.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dde.bjfxy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aqd.fengsongda.top

Java: // 手写递归
来源：http://inu.zhongyouzk.top

Go:   // 手写递归
来源：http://ano.zhoulong.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dtz.hnqzz.top

C#:   // 手写递归
来源：http://vgh.yonumen.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hsu.fengsongda.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jfj.xylfe.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xbr.9152youxi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ymd.fehbvm.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dey.xziqi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qge.uphjek.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://epi.nanxuanxn.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kzz.0kj1m.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://llg.birdmap.top


<!-- 参考信息 -->