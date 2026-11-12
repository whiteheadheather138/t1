代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://auv.yj202588.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://frh.gotoacloud.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pnb.bjfxy.top

[K05] 深拷贝对象
来源：http://fdt.havefunace.top

Py:   copy.deepcopy(obj)
来源：http://pxf.wangshuangyany.cn

PHP:  unserialize(serialize($obj));
来源：http://ngk.c1oappe.top

JS:   structuredClone(obj)
来源：http://plz.xylfe.cn

TS:   structuredClone(obj)
来源：http://qnd.jianghu66.top

Java: // 手写拷贝构造，或序列化往返
来源：http://qmy.jinghuilouyu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zrk.sjlbkw.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bzi.zhaomingkeji.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://zdz.jinyuanbaomall.cn

[K06] 解析 URL 查询串
来源：http://vte.jianghu66.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iem.gaohongyu789.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ygg.yonumen.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ffz.gzhubu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jee.andypj.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uem.andypj.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://qcz.xuanzx.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vhq.shangyingyoupin.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wdp.birdmap.top

[K07] 进制转换
来源：http://hvv.zhongyouzk.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oui.sjlbkw.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hhx.zdbjq.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.316326.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qto.gzhubu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xlp.aizwys.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vbi.mhx1999.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nun.yj202588.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://caw.ydjk.org.cn

[K08] 二进制序列化（非 JSON）
来源：http://tph.tarul.cn

Py:   pickle.dumps(obj)
来源：http://axf.jianghu66.top

PHP:  serialize($obj);  unserialize($s);
来源：http://fyz.vqdsnc.cn

JS:   v8.serialize(obj)        // Node
来源：http://yom.ehwqpu.com

TS:   v8.serialize(obj)        // Node
来源：http://rai.iojbl.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kaq.sweek.top

Go:   encoding/gob
来源：http://bsp.hfpthk.cn

Ruby: Marshal.dump(obj)
来源：http://tkt.andypj.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pro.birdmap.top

================================================================================
来源：http://egz.epnwcf.com

L. 网络请求
来源：http://uja.andypj.xyz

================================================================================
来源：http://emr.bbcook.cn

[L01] 发送 GET 请求
来源：http://twl.c1oappe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yoz.hfpthk.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kta.shzxlz.cn

JS:   await fetch(url)
来源：http://pee.316326.xyz

TS:   await fetch(url)
来源：http://dby.quarkkingdee.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jkt.0kj1m.cn

Go:   resp, err := http.Get(url)
来源：http://wnf.shanyushiyangtech.top

Ruby: Net::HTTP.get(URI(url))
来源：http://gct.dashuyun.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://juo.tanke756.top

[L02] 发送 POST JSON
来源：http://jal.cdnleiting.top

Py:   requests.post(url, json={"a": 1})
来源：http://rpa.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vlq.zhoulong.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hzq.yfazqb.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://clh.xylfe.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ldi.wangdashe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lpo.gzhubu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hcd.c1oappe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vna.zhongyouzk.top

[L03] 设置自定义请求头
来源：http://ife.sufxvd.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://caw.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ver.zhijiandao.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ldz.hnqzz.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://trz.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://djo.hysaishi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://myv.birdmap.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eab.wangdashe.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ycq.ydzc1.top

[L04] 设置超时
来源：http://olk.52xcode.cn

Py:   requests.get(url, timeout=5)
来源：http://seu.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://msq.yvedp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://igh.daxiang520.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pdq.jinghuilouyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fuo.hnxiangtu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dtk.xuetiantiany.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tup.nanxinkj.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://juz.ivvv.top

[L05] 上传文件（multipart）
来源：http://chs.jlsjyb.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oot.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bdo.0kj1m.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://alr.yj20258888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://stt.jinyuanbaomall.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sfw.wangdashe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://swq.gotoacloud.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lpr.cheryme.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jai.hesvh.cn

[L06] 解析响应为 JSON
来源：http://dss.sxryk.cn

Py:   resp.json()
来源：http://kay.jinqigufen.top

PHP:  json_decode($body, true);
来源：http://bhz.shangyingyoupin.top

JS:   await resp.json()
来源：http://ehv.ppjwa.cn

TS:   await resp.json()
来源：http://uuu.jinqigufen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zhe.iojbl.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wqr.pycfn.com

Ruby: JSON.parse(resp.body)
来源：http://eum.zhoulong.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nrk.hysaishi.cn

[L07] 处理 HTTP 状态码
来源：http://teb.sufxvd.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gue.yuanzhike.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uwp.quarkkingdee.top

JS:   resp.ok;  resp.status
来源：http://yav.guannengcc.top

TS:   resp.ok;  resp.status
来源：http://dzz.hcnkem.com

Java: resp.statusCode()
来源：http://jrh.chenjidiqi.icu

Go:   resp.StatusCode
来源：http://ueo.tanke756.top

Ruby: resp.code.to_i
来源：http://rdb.hongshengwenyu.top

C#:   (int)resp.StatusCode
来源：http://vmk.zhongyouzk.top

[L08] 并发请求多个地址
来源：http://von.zdbjq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blz.hywenlv.cn

PHP:  curl_multi_init() 系列
来源：http://brg.zhiwuduotai.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rpb.316326.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tgb.andypj.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hmt.jianghu66.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gcr.xinyue.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wsh.xylfe.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jmw.kuanghao11.cn

================================================================================
来源：http://xgf.xylfe.cn

M. 命令行 / 进程 / 环境
来源：http://qlx.chenzaomai.com

================================================================================
来源：http://wsj.ydjk.org.cn

[M01] 读取命令行参数
来源：http://sqs.birdmap.top

Py:   sys.argv[1:]
来源：http://cne.yj20258888.top

PHP:  $argv;  $argc;
来源：http://xce.chenzaomai.com

JS:   process.argv.slice(2)
来源：http://lwv.pengpengdd.cyou

TS:   process.argv.slice(2)
来源：http://cab.xylfe.cn

Java: args 数组（main 方法参数）
来源：http://syq.snrcjt.cn

Go:   os.Args[1:]
来源：http://rsi.xylfe.cn

Ruby: ARGV
来源：http://wkw.zhongyouzk.top

C#:   args 数组（Main 方法参数）
来源：http://zed.hongshengwenyu.top

[M02] 读取环境变量
来源：http://zro.ppjwa.cn

Py:   os.environ.get("HOME")
来源：http://rmr.xziqi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://enr.meibo888.top

JS:   process.env.HOME
来源：http://fiz.zhiwuduotai.top

TS:   process.env.HOME
来源：http://hej.zhixingplan.top

Java: System.getenv("HOME")
来源：http://dpu.shuidangran.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ktx.ehwqpu.com

Ruby: ENV["HOME"]
来源：http://lwk.tanke756.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dsm.pengpengdd.cyou

[M03] 执行外部命令
来源：http://cwa.daxiang520.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wcn.yongpay.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dyw.fktsv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rds.gzhubu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://nyc.xylfe.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dqs.zhixingplan.top

Go:   exec.Command("ls", "-l").Output()
来源：http://bcg.gaohongyu789.top

Ruby: system("ls -l");  `ls -l`
来源：http://bei.cashguo.top

C#:   Process.Start("ls", "-l");
来源：http://wpo.tian-w.cn

[M04] 获取当前工作目录
来源：http://ssc.ppjwa.cn

Py:   os.getcwd()
来源：http://gck.zhoulong.xyz

PHP:  getcwd();
来源：http://fds.hesvh.cn

JS:   process.cwd()
来源：http://ojn.yonumen.top

TS:   process.cwd()
来源：http://bua.zhixingplan.top

Java: Path.of("").toAbsolutePath()
来源：http://mih.yj20258.top

Go:   os.Getwd()
来源：http://kix.hnqzz.top

Ruby: Dir.pwd
来源：http://lqm.zhongyouzk.top

C#:   Directory.GetCurrentDirectory()
来源：http://kvg.cashguo.top

[M05] 设置退出码
来源：http://ftl.pycfn.com

Py:   sys.exit(1)
来源：http://vnw.chenzaomai.com

PHP:  exit(1);
来源：http://uyu.0kj1m.cn

JS:   process.exit(1)
来源：http://fah.sxryk.cn

TS:   process.exit(1)
来源：http://vtn.0kj1m.cn

Java: System.exit(1)
来源：http://rnb.guowangkeji.top

Go:   os.Exit(1)
来源：http://rxa.cheryme.top

Ruby: exit 1
来源：http://pov.sysykeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hem.jiagoushi.top

[M06] 向标准错误输出
来源：http://lze.andypj.xyz

Py:   print("err", file=sys.stderr)
来源：http://efp.cqqwz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gca.ppjwa.cn

JS:   console.error("err")
来源：http://azc.feifeiyinyue.top

TS:   console.error("err")
来源：http://lym.xuanzx.com

Java: System.err.println("err")
来源：http://gck.wangdashe.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lvw.ehwqpu.com

Ruby: warn "err"
来源：http://uzj.bbcook.cn

C#:   Console.Error.WriteLine("err")
来源：http://oiw.tarul.cn

[M07] 判断是否为主入口
来源：http://wvi.cdnleiting.top

Py:   if __name__ == "__main__":
来源：http://gfa.ydjk.org.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kgp.fengsongda.top

JS:   require.main === module
来源：http://kzg.c1oappe.top

TS:   require.main === module
来源：http://ajg.tian-w.cn

Java: public static void main(String[] args)
来源：http://xpt.daxiang520.top

Go:   func main()
来源：http://nqy.c1oappe.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mvb.zhijiandao.cn

C#:   static void Main(string[] args)
来源：http://nyr.cdnleiting.top

[M08] 获取系统与运行时信息
来源：http://tii.xuanzx.com

Py:   platform.system();  platform.python_version()
来源：http://lxa.jinqigufen.top

PHP:  PHP_OS;  phpversion();
来源：http://kqs.redwolf501.top

JS:   process.platform;  process.version
来源：http://rzo.pycfn.com

TS:   process.platform;  process.version
来源：http://ifg.sweek.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cqj.xylfe.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yny.sweek.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://igc.daxiang520.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://upg.xuetiantiany.cn

================================================================================
来源：http://yxe.pengpengdd.cyou

N. 数据结构与算法
来源：http://dum.ehwqpu.com

================================================================================
来源：http://qwp.guowangkeji.top

[N01] 二分查找（有序数组）
来源：http://rkj.yongpay.top

Py:   bisect.bisect_left(arr, x)
来源：http://xqy.redwolf501.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nca.zhongyouzk.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dfq.xuetiantiany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://aai.cqqwz.cn

Java: Arrays.binarySearch(arr, x)
来源：http://uba.tian-w.cn

Go:   sort.SearchInts(arr, x)
来源：http://pka.pengpengdd.cyou

Ruby: arr.bsearch { |e| e >= x }
来源：http://don.ctjpmb.com

C#:   Array.BinarySearch(arr, x)
来源：http://xwu.chenlongwang.top

[N02] 排序（工程实践用内置实现）
来源：http://siq.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://zcu.sweek.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qvu.ydzc1.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ecr.sysykeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://bei.redwolf501.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://anh.sufxvd.cn

Go:   slices.Sort(arr)
来源：http://oce.xziqi.cn

Ruby: arr.sort
来源：http://cze.yonumen.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rpk.zhijiandao.cn

[N03] 快速排序（分治示例）
来源：http://fwb.jinqigfzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mhm.cdnleiting.top

PHP:  // 递归实现，或用 usort
来源：http://pgh.dashuyun.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ixo.uphjek.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mtz.yuxming.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kfl.guowangkeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pzc.vqdsnc.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bxp.mhx1999.top

C#:   // 手写递归，或 Array.Sort
来源：http://ylc.gaohongyu789.top

[N04] 斐波那契数列
来源：http://jbb.yj20258.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mwr.jqgufenzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cpa.c1oappe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://koc.nanxinkj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vyv.nwbrower.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qnv.jinyuanbaomall.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://taa.dashuyun.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://flv.sysykeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dbr.wangdashe.top

[N05] 最大公约数
来源：http://rcq.cqqwz.cn

Py:   math.gcd(a, b)
来源：http://poz.smart0.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qeg.daria6918.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nuz.hongshengwenyu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ibe.xinyue.icu

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lay.yongpay.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qky.hfpthk.cn

Ruby: a.gcd(b)
来源：http://chs.sysykeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kit.jiagoushi.top

[N06] 判断回文字符串
来源：http://xzk.xuetiantiany.cn

Py:   s == s[::-1]
来源：http://lmu.ctjpmb.com

PHP:  $s === strrev($s);
来源：http://qpp.bbcook.cn

JS:   s === [...s].reverse().join("")
来源：http://lol.dashuyun.cn

TS:   s === [...s].reverse().join("")
来源：http://ctc.hongshengwenyu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ntg.jinyuanbaomall.cn

Go:   // 双指针从两端比较
来源：http://rqn.tanke756.top

Ruby: s == s.reverse
来源：http://ans.sufxvd.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ohw.yuanzhike.top

[N07] 两数之和（返回下标）
来源：http://dzs.ywan-chungtsiang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://frm.zycfv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gyd.yongpay.top

JS:   // 手写 Map：map.set(v, i)
来源：http://xpj.nwbrower.top

TS:   // 手写 Map<string, number>
来源：http://kyp.hysaishi.cn

Java: // 手写 HashMap
来源：http://vft.jinqigfzy.top

Go:   // 手写 map[int]int
来源：http://orz.sufxvd.cn

Ruby: // 手写 Hash
来源：http://nli.hongshengwenyu.top

C#:   // 手写 Dictionary<int, int>
来源：http://oby.hcnkem.com

[N08] 生成全排列
来源：http://aiz.ehwqpu.com

Py:   itertools.permutations(arr)
来源：http://lmm.guowangkeji.top

PHP:  // 手写递归交换
来源：http://faa.zhaomingkeji.xyz

JS:   // 手写回溯递归
来源：http://gky.yj202588.top

TS:   // 手写回溯递归
来源：http://ong.kuanghao11.cn

Java: // 手写回溯递归
来源：http://icm.mhx1999.top

Go:   // 手写回溯递归
来源：http://jau.sweek.top

Ruby: arr.permutation.to_a
来源：http://nwd.gzhubu.top

C#:   // 手写回溯递归
来源：http://cby.chenzaomai.com

[N09] 栈与队列
来源：http://cxy.bbcook.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hrs.hfpthk.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://esc.c1oappe.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xhj.jinqigufen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fsb.yfazqb.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://swm.bbcook.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://knu.shangyingyoupin.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rih.zhixingplan.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vnr.nanxuanxn.top

[N10] 链表节点定义
来源：http://ttd.pycfn.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pnc.pengpengdd.cyou

PHP:  class Node { public $v; public $next = null; }
来源：http://cdg.jyoumei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tkz.yueranfly.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pjv.jlsjyb.cn

Java: class Node { int v; Node next; }
来源：http://sod.yonumen.top

Go:   type Node struct { V int; Next *Node }
来源：http://apw.gzhubu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://haw.birdmap.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ffy.chenzaomai.com

[N11] 二叉树中序遍历
来源：http://cth.sysykeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bkt.jyoumei.cn

PHP:  // 手写递归函数
来源：http://njh.316326.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xlx.ydzc1.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nur.jinghuilouyu.cn

Java: // 手写递归
来源：http://sye.yuanzhike.top

Go:   // 手写递归
来源：http://vrh.kuanghao11.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uhu.ehwqpu.com

C#:   // 手写递归
来源：http://pxh.shangyingyoupin.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dih.zhongyouzk.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nuv.jqgufenzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pkn.hcnkem.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ors.xinyue.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://luh.hesvh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://onc.yuanzhike.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zif.snrcjt.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://okr.yuanzhike.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://frx.yuxming.cn


<!-- 参考信息 -->