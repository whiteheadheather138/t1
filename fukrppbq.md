代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://tmg.316326.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://chv.sweek.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nwo.xziqi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pkr.chenzaomai.com

Ruby: JSON.pretty_generate(obj)
来源：http://qae.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://aoy.nwbrower.top

[K04] 读取 JSON 文件
来源：http://ktw.zhongyouzk.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://neo.feifeiyinyue.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nyc.yuanzhike.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://avj.hammf.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mel.hfpthk.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rnf.cashguo.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zmo.tianlin.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://opw.wangdashe.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://seh.yuxming.cn

[K05] 深拷贝对象
来源：http://lvv.pengpengdd.cyou

Py:   copy.deepcopy(obj)
来源：http://usc.jinyuanbaomall.cn

PHP:  unserialize(serialize($obj));
来源：http://pdl.fehbvm.com

JS:   structuredClone(obj)
来源：http://nna.zdbjq.cn

TS:   structuredClone(obj)
来源：http://vyf.cashguo.top

Java: // 手写拷贝构造，或序列化往返
来源：http://cek.xuetiantiany.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bxn.jyoumei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qct.fehbvm.com

C#:   // 序列化往返，或自定义 Clone
来源：http://til.yj202588.top

[K06] 解析 URL 查询串
来源：http://nwh.redwolf501.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kcx.snrcjt.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://aar.cashguo.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jzl.redwolf501.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gru.hywenlv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dxz.fehbvm.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://vzs.sysykeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ukm.hfpthk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hln.tianlin.xyz

[K07] 进制转换
来源：http://mtz.fktsv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nwl.xuetiantiany.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ixp.ivvv.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rcp.jinqigufen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jat.zhengqikj.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xro.jlsjyb.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iqy.smart0.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sfm.vehdjk.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://asq.daria6918.cn

[K08] 二进制序列化（非 JSON）
来源：http://rww.mhx1999.top

Py:   pickle.dumps(obj)
来源：http://wwu.hnxiangtu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://yca.cheryme.top

JS:   v8.serialize(obj)        // Node
来源：http://qvo.cheryme.top

TS:   v8.serialize(obj)        // Node
来源：http://yyk.shanyushiyangtech.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pbr.chenlongwang.top

Go:   encoding/gob
来源：http://qwx.jianghu66.top

Ruby: Marshal.dump(obj)
来源：http://jql.yj20258.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ofk.xylfe.cn

================================================================================
来源：http://pao.shzxlz.cn

L. 网络请求
来源：http://ait.hysaishi.cn

================================================================================
来源：http://fhr.tianlin.xyz

[L01] 发送 GET 请求
来源：http://mpq.hcnkem.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yzb.smart0.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gpp.hysaishi.cn

JS:   await fetch(url)
来源：http://alx.dashuyun.cn

TS:   await fetch(url)
来源：http://jnd.gzhubu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wdc.yonumen.top

Go:   resp, err := http.Get(url)
来源：http://yab.jlsjyb.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zkk.bjfxy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://esb.xingfuxueyuan.xyz

[L02] 发送 POST JSON
来源：http://cgj.yonumen.top

Py:   requests.post(url, json={"a": 1})
来源：http://drw.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pwm.bbcook.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bll.ivvv.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ntz.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qnf.tarul.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://idd.pycfn.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aqb.xuanzx.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://evb.ydjk.org.cn

[L03] 设置自定义请求头
来源：http://ewv.52xcode.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ijz.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ctc.wangshuangyany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wac.havefunace.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aqw.hcnkem.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wsd.gogol.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ngx.ydzc1.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gic.jianghu66.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yrb.shzxlz.cn

[L04] 设置超时
来源：http://wqh.mhx1999.top

Py:   requests.get(url, timeout=5)
来源：http://sne.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uav.dianchejie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zxq.jqgfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yqt.jinghuilouyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gga.aizwys.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hyj.pycfn.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uxi.chenzaomai.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xpn.sufxvd.cn

[L05] 上传文件（multipart）
来源：http://qcz.yonumen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zan.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://eyq.yuanzhike.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hhl.tian-w.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dad.xuetiantiany.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hcx.yongpay.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://whb.vqdsnc.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eav.smart0.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://odl.xuetiantiany.cn

[L06] 解析响应为 JSON
来源：http://oaz.yueranfly.top

Py:   resp.json()
来源：http://ghr.pycfn.com

PHP:  json_decode($body, true);
来源：http://zyn.ctjpmb.com

JS:   await resp.json()
来源：http://ssf.jyoumei.cn

TS:   await resp.json()
来源：http://tsw.sweek.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eyg.tianlin.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kvl.hfpthk.cn

Ruby: JSON.parse(resp.body)
来源：http://gao.zhoulong.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vxc.jinqigfzy.top

[L07] 处理 HTTP 状态码
来源：http://gpx.cqqwz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zja.sufxvd.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wse.sjlbkw.cn

JS:   resp.ok;  resp.status
来源：http://xvc.hywenlv.cn

TS:   resp.ok;  resp.status
来源：http://dsc.yuxming.cn

Java: resp.statusCode()
来源：http://cdu.nanxinkj.top

Go:   resp.StatusCode
来源：http://wqq.fehbvm.com

Ruby: resp.code.to_i
来源：http://qyr.wangshuangyany.cn

C#:   (int)resp.StatusCode
来源：http://rbp.wangshuangyany.cn

[L08] 并发请求多个地址
来源：http://kpb.vehdjk.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wbp.dianchejie.cn

PHP:  curl_multi_init() 系列
来源：http://cdv.sjlbkw.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://swj.xziqi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uut.wangshuangyany.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uaj.yanxiufei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pgp.hcnkem.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zwd.ctjpmb.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://isr.52xcode.cn

================================================================================
来源：http://qgi.jqgfzy.top

M. 命令行 / 进程 / 环境
来源：http://qnt.zdqjudy.top

================================================================================
来源：http://siz.xuetiantiany.cn

[M01] 读取命令行参数
来源：http://lam.fzhhl.top

Py:   sys.argv[1:]
来源：http://yll.daria6918.cn

PHP:  $argv;  $argc;
来源：http://cfu.316326.xyz

JS:   process.argv.slice(2)
来源：http://hyy.xinyue.icu

TS:   process.argv.slice(2)
来源：http://apb.quarkkingdee.top

Java: args 数组（main 方法参数）
来源：http://ufc.nanxinkj.top

Go:   os.Args[1:]
来源：http://ths.jiagoushi.top

Ruby: ARGV
来源：http://urz.jinqigfzy.top

C#:   args 数组（Main 方法参数）
来源：http://lqb.ywan-chungtsiang.top

[M02] 读取环境变量
来源：http://axq.ywan-chungtsiang.top

Py:   os.environ.get("HOME")
来源：http://plj.xziqi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gur.c1oappe.top

JS:   process.env.HOME
来源：http://dnu.andypj.xyz

TS:   process.env.HOME
来源：http://pun.sweek.top

Java: System.getenv("HOME")
来源：http://kjh.kuanghao11.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yph.bjfxy.top

Ruby: ENV["HOME"]
来源：http://kni.chenlongwang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://eri.guowangkeji.top

[M03] 执行外部命令
来源：http://xnh.aibaodan.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yfl.xuetiantiany.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cdo.yfazqb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://pic.cucudq.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rki.uphjek.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://diz.shanyushiyangtech.top

Go:   exec.Command("ls", "-l").Output()
来源：http://kjr.yj202588.top

Ruby: system("ls -l");  `ls -l`
来源：http://qtu.yvedp.cn

C#:   Process.Start("ls", "-l");
来源：http://bfs.hongshengwenyu.top

[M04] 获取当前工作目录
来源：http://zfp.chenjidiqi.icu

Py:   os.getcwd()
来源：http://qmg.sufxvd.cn

PHP:  getcwd();
来源：http://lmv.yj202588.top

JS:   process.cwd()
来源：http://yme.jiagoushi.top

TS:   process.cwd()
来源：http://ukh.jianghu66.top

Java: Path.of("").toAbsolutePath()
来源：http://lbg.316326.xyz

Go:   os.Getwd()
来源：http://vge.fehbvm.com

Ruby: Dir.pwd
来源：http://jbz.ehwqpu.com

C#:   Directory.GetCurrentDirectory()
来源：http://mon.gogol.net.cn

[M05] 设置退出码
来源：http://ati.iojbl.cn

Py:   sys.exit(1)
来源：http://aea.hnxiangtu.top

PHP:  exit(1);
来源：http://npo.cqqwz.cn

JS:   process.exit(1)
来源：http://ukx.yuxming.cn

TS:   process.exit(1)
来源：http://duh.gaohongyu789.top

Java: System.exit(1)
来源：http://itm.sweek.top

Go:   os.Exit(1)
来源：http://gnd.fktsv.cn

Ruby: exit 1
来源：http://lpm.ppjwa.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nvu.yangfankeji.com

[M06] 向标准错误输出
来源：http://sbw.sjlbkw.cn

Py:   print("err", file=sys.stderr)
来源：http://seh.wangdashe.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bwu.xziqi.cn

JS:   console.error("err")
来源：http://htu.shzxlz.cn

TS:   console.error("err")
来源：http://coa.aizwys.cn

Java: System.err.println("err")
来源：http://hlr.cheryme.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://inw.hywenlv.cn

Ruby: warn "err"
来源：http://ijm.uphjek.com

C#:   Console.Error.WriteLine("err")
来源：http://mub.haohaochexian.top

[M07] 判断是否为主入口
来源：http://dsy.pycfn.com

Py:   if __name__ == "__main__":
来源：http://ftj.yanxiufei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://amp.xinyue.icu

JS:   require.main === module
来源：http://vqz.shanyushiyangtech.top

TS:   require.main === module
来源：http://wrf.sweek.top

Java: public static void main(String[] args)
来源：http://pza.hammf.cn

Go:   func main()
来源：http://hvf.birdmap.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://men.c1oappe.top

C#:   static void Main(string[] args)
来源：http://czg.quarkkingdee.top

[M08] 获取系统与运行时信息
来源：http://egz.jinyuanbaomall.cn

Py:   platform.system();  platform.python_version()
来源：http://yxk.xingfuxueyuan.xyz

PHP:  PHP_OS;  phpversion();
来源：http://lnx.nanxuanxn.top

JS:   process.platform;  process.version
来源：http://tld.sjlbkw.cn

TS:   process.platform;  process.version
来源：http://qky.andypj.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zyx.fktsv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://oqr.feifeiyinyue.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://klx.yangfankeji.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://nkb.316326.xyz

================================================================================
来源：http://zwn.ydzc1.top

N. 数据结构与算法
来源：http://vqn.tian-w.cn

================================================================================
来源：http://php.ybcxt.top

[N01] 二分查找（有序数组）
来源：http://oew.zdqjudy.top

Py:   bisect.bisect_left(arr, x)
来源：http://fhz.zhaomingkeji.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lyj.c1oappe.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lgy.gaohongyu789.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ati.fktsv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://eak.yvedp.cn

Go:   sort.SearchInts(arr, x)
来源：http://fow.yuxming.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yfv.yuxming.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zjq.xuetiantiany.cn

[N02] 排序（工程实践用内置实现）
来源：http://upz.hammf.cn

Py:   sorted(arr);  arr.sort()
来源：http://rat.andypj.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lei.fanxiaobao.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://rmx.0kj1m.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pbf.tian-w.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://aab.yvedp.cn

Go:   slices.Sort(arr)
来源：http://isd.fanxiaobao.xyz

Ruby: arr.sort
来源：http://lpy.ybcxt.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://dyn.gogol.net.cn

[N03] 快速排序（分治示例）
来源：http://uhq.yangfankeji.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rsi.svipenyu.cn

PHP:  // 递归实现，或用 usort
来源：http://tdh.ehwqpu.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ibg.cucudq.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://urq.cucudq.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://znf.feifeiyinyue.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nvi.tanke756.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wsj.epnwcf.com

C#:   // 手写递归，或 Array.Sort
来源：http://qoc.haohaochexian.top

[N04] 斐波那契数列
来源：http://ghk.tian-w.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jah.aizwys.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://eve.guannengcc.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pjr.zhiwuduotai.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://asf.zhoulong.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ika.cqqwz.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pkq.guannengcc.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ewy.ivvv.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fkp.jinghuilouyu.cn

[N05] 最大公约数
来源：http://pab.bjfxy.top

Py:   math.gcd(a, b)
来源：http://svs.zhaomingkeji.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sfj.yj20258888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://avu.cheryme.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://apq.ppjwa.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wot.xuanzx.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://svn.9152youxi.cn

Ruby: a.gcd(b)
来源：http://wfn.ehwqpu.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zub.ivvv.top

[N06] 判断回文字符串
来源：http://yiw.jiagoushi.top

Py:   s == s[::-1]
来源：http://yeo.dashuyun.cn

PHP:  $s === strrev($s);
来源：http://cxj.fengsongda.top

JS:   s === [...s].reverse().join("")
来源：http://mre.zhoulong.xyz

TS:   s === [...s].reverse().join("")
来源：http://mha.yanxiufei.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xec.jinqigfzy.top

Go:   // 双指针从两端比较
来源：http://ozd.epnwcf.com

Ruby: s == s.reverse
来源：http://oif.vehdjk.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://bpt.aizwys.cn

[N07] 两数之和（返回下标）
来源：http://xol.iojbl.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://duj.tanke756.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lzh.cdnleiting.top

JS:   // 手写 Map：map.set(v, i)
来源：http://oma.yuxming.cn

TS:   // 手写 Map<string, number>
来源：http://pjj.haohaochexian.top

Java: // 手写 HashMap
来源：http://plq.xingfuxueyuan.xyz

Go:   // 手写 map[int]int
来源：http://ohs.cqqwz.cn

Ruby: // 手写 Hash
来源：http://jdw.cqqwz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gcl.yvedp.cn

[N08] 生成全排列
来源：http://yfg.ehwqpu.com

Py:   itertools.permutations(arr)
来源：http://fgq.xinyue.icu

PHP:  // 手写递归交换
来源：http://bob.sweek.top

JS:   // 手写回溯递归
来源：http://rxf.tanke756.top

TS:   // 手写回溯递归
来源：http://lxt.zdqjudy.top

Java: // 手写回溯递归
来源：http://yyy.dianchejie.cn

Go:   // 手写回溯递归
来源：http://ixd.tanke756.top

Ruby: arr.permutation.to_a
来源：http://sfp.yfazqb.com

C#:   // 手写回溯递归
来源：http://xar.shuidangran.top

[N09] 栈与队列
来源：http://hmi.gotoacloud.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://iat.sufxvd.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tnf.hongshengwenyu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wpf.ybcxt.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://byi.pengpengdd.cyou

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blu.chenzaomai.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://whb.hesvh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://eoa.yongpay.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bvt.birdmap.top

[N10] 链表节点定义
来源：http://gmx.birdmap.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jsz.yj20258.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ssw.andypj.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lcq.cdnleiting.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qpm.zhiwuduotai.top

Java: class Node { int v; Node next; }
来源：http://wwb.meibo888.top

Go:   type Node struct { V int; Next *Node }
来源：http://zbu.pycfn.com

Ruby: Node = Struct.new(:v, :next)
来源：http://nxk.nwbrower.top

C#:   class Node { public int V; public Node? Next; }
来源：http://qdt.hcnkem.com

[N11] 二叉树中序遍历
来源：http://jcf.pengpengdd.cyou

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zrm.havefunace.top

PHP:  // 手写递归函数
来源：http://dbz.daria6918.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://law.nanxinkj.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pls.hongshengwenyu.top

Java: // 手写递归
来源：http://ill.gogol.net.cn


<!-- 参考信息 -->