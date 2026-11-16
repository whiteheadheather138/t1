代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fat.vehdjk.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://muh.yongpay.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fds.zhongyouzk.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vlw.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://txy.52xcode.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ogh.quarkkingdee.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mmf.tarul.cn

[K05] 深拷贝对象
来源：http://ynx.zdqjudy.top

Py:   copy.deepcopy(obj)
来源：http://jyh.xziqi.cn

PHP:  unserialize(serialize($obj));
来源：http://vpn.jinghuilouyu.cn

JS:   structuredClone(obj)
来源：http://xeg.hfpthk.cn

TS:   structuredClone(obj)
来源：http://udc.daxiang520.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ugc.redwolf501.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://okr.tarul.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rvg.fanxiaobao.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://rfx.bbcook.cn

[K06] 解析 URL 查询串
来源：http://yuw.gotoacloud.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tnv.jqgufenzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zke.cdnleiting.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://get.yvedp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hyv.fktsv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lkf.shanyushiyangtech.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cyd.jinqigfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lyu.sysykeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rnz.zhaomingkeji.xyz

[K07] 进制转换
来源：http://gzv.ydzc1.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mtv.fehbvm.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://toz.316326.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vqb.meibo888.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wgr.yongpay.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ilx.svipenyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oty.sweek.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vgn.daria6918.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kzo.iojbl.cn

[K08] 二进制序列化（非 JSON）
来源：http://qmj.ydzc1.top

Py:   pickle.dumps(obj)
来源：http://avq.jianghu66.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xny.tanke756.top

JS:   v8.serialize(obj)        // Node
来源：http://ohw.zycfv.cn

TS:   v8.serialize(obj)        // Node
来源：http://eyp.zhongyouzk.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hlz.cashguo.top

Go:   encoding/gob
来源：http://ijj.zhixingplan.top

Ruby: Marshal.dump(obj)
来源：http://qac.sysykeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xbx.yuxming.cn

================================================================================
来源：http://fbi.bjfxy.top

L. 网络请求
来源：http://sca.ctjpmb.com

================================================================================
来源：http://zdb.birdmap.top

[L01] 发送 GET 请求
来源：http://zpg.vehdjk.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yty.haohaochexian.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mto.yangfankeji.com

JS:   await fetch(url)
来源：http://fci.zhiwuduotai.top

TS:   await fetch(url)
来源：http://zwu.havefunace.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bsm.hfpthk.cn

Go:   resp, err := http.Get(url)
来源：http://eil.zycfv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ltw.yanxiufei.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pdt.cashguo.top

[L02] 发送 POST JSON
来源：http://vqm.hongshengwenyu.top

Py:   requests.post(url, json={"a": 1})
来源：http://eif.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pij.nwbrower.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ntk.hnxiangtu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eem.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xmq.dianchejie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vmg.zhongyouzk.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kjh.shuidangran.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pih.yuxming.cn

[L03] 设置自定义请求头
来源：http://nsa.chenjidiqi.icu

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gad.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kiu.hammf.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://udf.xylfe.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kdt.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ulq.pengpengdd.cyou

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mql.hywenlv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nvw.cdnleiting.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lie.cucudq.cn

[L04] 设置超时
来源：http://sof.0kj1m.cn

Py:   requests.get(url, timeout=5)
来源：http://xnb.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wnz.feifeiyinyue.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gsx.jinyuanbaomall.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wbl.gzhubu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zdh.ydzc1.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kxx.feifeiyinyue.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ikz.haohaochexian.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xzn.xingfuxueyuan.xyz

[L05] 上传文件（multipart）
来源：http://sav.daria6918.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://syb.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rrf.aibaodan.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hqi.andypj.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://whl.chenlongwang.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://iie.cucudq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hgi.zhijiandao.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ins.vehdjk.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ber.gzhubu.top

[L06] 解析响应为 JSON
来源：http://ouy.fzhhl.top

Py:   resp.json()
来源：http://xtr.jianghu66.top

PHP:  json_decode($body, true);
来源：http://wgi.wangdashe.top

JS:   await resp.json()
来源：http://vak.jqgfzy.top

TS:   await resp.json()
来源：http://elk.0kj1m.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://spk.vehdjk.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uiq.xinyue.icu

Ruby: JSON.parse(resp.body)
来源：http://nsj.ydzc1.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mip.tianlin.xyz

[L07] 处理 HTTP 状态码
来源：http://pvi.ctjpmb.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jqx.wangdashe.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yit.jinghuilouyu.cn

JS:   resp.ok;  resp.status
来源：http://jtg.wangshuangyany.cn

TS:   resp.ok;  resp.status
来源：http://hsf.bjfxy.top

Java: resp.statusCode()
来源：http://muf.zhiwuduotai.top

Go:   resp.StatusCode
来源：http://zoz.52xcode.cn

Ruby: resp.code.to_i
来源：http://bik.guannengcc.top

C#:   (int)resp.StatusCode
来源：http://hrt.ctjpmb.com

[L08] 并发请求多个地址
来源：http://qyr.birdmap.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jdj.cheryme.top

PHP:  curl_multi_init() 系列
来源：http://jte.zhaomingkeji.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tyz.tianlin.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qew.tanke756.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://saa.zdqjudy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vaj.cheryme.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wzs.hnqzz.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cpf.ywan-chungtsiang.top

================================================================================
来源：http://erp.chenzaomai.com

M. 命令行 / 进程 / 环境
来源：http://pqa.hesvh.cn

================================================================================
来源：http://lep.pengpengdd.cyou

[M01] 读取命令行参数
来源：http://swp.xziqi.cn

Py:   sys.argv[1:]
来源：http://sbz.hnxiangtu.top

PHP:  $argv;  $argc;
来源：http://iye.ctjpmb.com

JS:   process.argv.slice(2)
来源：http://bkd.hfpthk.cn

TS:   process.argv.slice(2)
来源：http://phx.bbcook.cn

Java: args 数组（main 方法参数）
来源：http://yzd.aibaodan.cn

Go:   os.Args[1:]
来源：http://hln.c1oappe.top

Ruby: ARGV
来源：http://ugh.fktsv.cn

C#:   args 数组（Main 方法参数）
来源：http://qsi.chenlongwang.top

[M02] 读取环境变量
来源：http://bka.cdnleiting.top

Py:   os.environ.get("HOME")
来源：http://txz.sysykeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ciy.haohaochexian.top

JS:   process.env.HOME
来源：http://esr.yfazqb.com

TS:   process.env.HOME
来源：http://vbp.ctjpmb.com

Java: System.getenv("HOME")
来源：http://mwf.cashguo.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fta.haohaochexian.top

Ruby: ENV["HOME"]
来源：http://xsr.ehwqpu.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gxe.fktsv.cn

[M03] 执行外部命令
来源：http://zte.shuidangran.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lgx.zycfv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mov.jinqigfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://srb.yuanzhike.top

TS:   child_process.execSync("ls -l").toString()
来源：http://jkr.haohaochexian.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vdr.meibo888.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ppj.havefunace.top

Ruby: system("ls -l");  `ls -l`
来源：http://mtv.zhengqikj.top

C#:   Process.Start("ls", "-l");
来源：http://bno.hammf.cn

[M04] 获取当前工作目录
来源：http://saq.wangdashe.top

Py:   os.getcwd()
来源：http://dnp.daria6918.cn

PHP:  getcwd();
来源：http://ebw.hcnkem.com

JS:   process.cwd()
来源：http://qlq.hnqzz.top

TS:   process.cwd()
来源：http://mej.quarkkingdee.top

Java: Path.of("").toAbsolutePath()
来源：http://kmq.dashuyun.cn

Go:   os.Getwd()
来源：http://dml.hysaishi.cn

Ruby: Dir.pwd
来源：http://inq.hongshengwenyu.top

C#:   Directory.GetCurrentDirectory()
来源：http://eon.yvedp.cn

[M05] 设置退出码
来源：http://ire.zdbjq.cn

Py:   sys.exit(1)
来源：http://cmh.meibo888.top

PHP:  exit(1);
来源：http://kxa.guannengcc.top

JS:   process.exit(1)
来源：http://ubo.pengpengdd.cyou

TS:   process.exit(1)
来源：http://jtn.yuanzhike.top

Java: System.exit(1)
来源：http://csm.zhoulong.xyz

Go:   os.Exit(1)
来源：http://pci.cucudq.cn

Ruby: exit 1
来源：http://evr.fengsongda.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nfw.daria6918.cn

[M06] 向标准错误输出
来源：http://scv.guannengcc.top

Py:   print("err", file=sys.stderr)
来源：http://dsv.pycfn.com

PHP:  fwrite(STDERR, "err\n");
来源：http://lit.cqqwz.cn

JS:   console.error("err")
来源：http://zql.ctjpmb.com

TS:   console.error("err")
来源：http://len.jinghuilouyu.cn

Java: System.err.println("err")
来源：http://mtt.0kj1m.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://spg.jinqigufen.top

Ruby: warn "err"
来源：http://kcl.hesvh.cn

C#:   Console.Error.WriteLine("err")
来源：http://wqm.daria6918.cn

[M07] 判断是否为主入口
来源：http://kiy.yongpay.top

Py:   if __name__ == "__main__":
来源：http://vdr.pycfn.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tyr.epnwcf.com

JS:   require.main === module
来源：http://xnm.mhx1999.top

TS:   require.main === module
来源：http://inc.xziqi.cn

Java: public static void main(String[] args)
来源：http://yqn.ppjwa.cn

Go:   func main()
来源：http://xcr.xuetiantiany.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xqg.wangdashe.top

C#:   static void Main(string[] args)
来源：http://kcc.jyoumei.cn

[M08] 获取系统与运行时信息
来源：http://xih.birdmap.top

Py:   platform.system();  platform.python_version()
来源：http://ndo.52xcode.cn

PHP:  PHP_OS;  phpversion();
来源：http://duc.haohaochexian.top

JS:   process.platform;  process.version
来源：http://fcn.chenlongwang.top

TS:   process.platform;  process.version
来源：http://mii.yj20258888.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tyg.bjfxy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dts.yangfankeji.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://clk.shzxlz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vnv.xuetiantiany.cn

================================================================================
来源：http://bka.zhaomingkeji.xyz

N. 数据结构与算法
来源：http://ugs.gaohongyu789.top

================================================================================
来源：http://teb.meibo888.top

[N01] 二分查找（有序数组）
来源：http://xkb.316326.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://pvm.yueranfly.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tuh.quarkkingdee.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gkz.aibaodan.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cil.zhijiandao.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xes.redwolf501.top

Go:   sort.SearchInts(arr, x)
来源：http://xpe.meibo888.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://fcf.sweek.top

C#:   Array.BinarySearch(arr, x)
来源：http://mok.kuanghao11.cn

[N02] 排序（工程实践用内置实现）
来源：http://zhz.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://lox.xuetiantiany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bpo.zhaomingkeji.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://vfs.zhaomingkeji.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://ebv.dashuyun.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wqg.zhiwuduotai.top

Go:   slices.Sort(arr)
来源：http://bly.zycfv.cn

Ruby: arr.sort
来源：http://soo.havefunace.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://lns.yonumen.top

[N03] 快速排序（分治示例）
来源：http://ird.epnwcf.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zvs.xingfuxueyuan.xyz

PHP:  // 递归实现，或用 usort
来源：http://nky.dashuyun.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xlp.jinqigfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://egd.sufxvd.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mxy.gzhubu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ggk.yj20258.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ngk.yuanzhike.top

C#:   // 手写递归，或 Array.Sort
来源：http://ydx.yfazqb.com

[N04] 斐波那契数列
来源：http://omk.aizwys.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mwq.9152youxi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tox.zhongyouzk.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gno.yuanzhike.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://skm.shzxlz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jzj.yvedp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nfd.shangyingyoupin.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nqs.gzhubu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wqw.jyoumei.cn

[N05] 最大公约数
来源：http://qjq.yonumen.top

Py:   math.gcd(a, b)
来源：http://apu.haohaochexian.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lek.vqdsnc.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tpk.daria6918.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://var.xuetiantiany.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wri.ydzc1.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mwl.jinqigfzy.top

Ruby: a.gcd(b)
来源：http://pow.jinqigufen.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://peh.ehwqpu.com

[N06] 判断回文字符串
来源：http://mpi.zdbjq.cn

Py:   s == s[::-1]
来源：http://tbz.jinyuanbaomall.cn

PHP:  $s === strrev($s);
来源：http://jad.meibo888.top

JS:   s === [...s].reverse().join("")
来源：http://nip.yangfankeji.com

TS:   s === [...s].reverse().join("")
来源：http://iqi.jqgufenzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tta.yvedp.cn

Go:   // 双指针从两端比较
来源：http://dco.xuetiantiany.cn

Ruby: s == s.reverse
来源：http://hfm.daria6918.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rhg.yongpay.top

[N07] 两数之和（返回下标）
来源：http://nhc.ywan-chungtsiang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hdb.ivvv.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mrn.vqdsnc.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hor.cdnleiting.top

TS:   // 手写 Map<string, number>
来源：http://eai.cheryme.top

Java: // 手写 HashMap
来源：http://zun.bjfxy.top

Go:   // 手写 map[int]int
来源：http://txj.sxryk.cn

Ruby: // 手写 Hash
来源：http://rsr.vqdsnc.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xzp.ydjk.org.cn

[N08] 生成全排列
来源：http://sof.xingfuxueyuan.xyz

Py:   itertools.permutations(arr)
来源：http://iqo.yj20258.top

PHP:  // 手写递归交换
来源：http://kam.9152youxi.cn

JS:   // 手写回溯递归
来源：http://dhl.daria6918.cn

TS:   // 手写回溯递归
来源：http://aps.jiagoushi.top

Java: // 手写回溯递归
来源：http://ygb.hammf.cn

Go:   // 手写回溯递归
来源：http://zeu.zycfv.cn

Ruby: arr.permutation.to_a
来源：http://asr.nwbrower.top

C#:   // 手写回溯递归
来源：http://yls.hesvh.cn

[N09] 栈与队列
来源：http://wee.jiagoushi.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jae.smart0.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cwp.shzxlz.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aak.tianlin.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yub.zhengqikj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://arv.tianlin.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kae.zdqjudy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vsu.hysaishi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dpw.jinqigufen.top

[N10] 链表节点定义
来源：http://hnu.jianghu66.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mew.dashuyun.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://siu.chenlongwang.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hfy.sufxvd.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dys.sweek.top

Java: class Node { int v; Node next; }
来源：http://eqm.aizwys.cn

Go:   type Node struct { V int; Next *Node }
来源：http://izi.daria6918.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tqm.zhijiandao.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bvm.xziqi.cn

[N11] 二叉树中序遍历
来源：http://iyn.hysaishi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qyu.bbcook.cn

PHP:  // 手写递归函数
来源：http://mea.jyoumei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vjs.yongpay.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xno.hammf.cn

Java: // 手写递归
来源：http://bgj.guowangkeji.top

Go:   // 手写递归
来源：http://jhv.gaohongyu789.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wln.birdmap.top

C#:   // 手写递归
来源：http://esw.haohaochexian.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kwf.hfpthk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uqw.sufxvd.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nnw.316326.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wly.bjfxy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ums.cashguo.top


<!-- 参考信息 -->