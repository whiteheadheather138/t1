代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ifu.yongpay.top

[K03] JSON 美化输出（带缩进）
来源：http://jdu.ehwqpu.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://guf.cucudq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vhu.chenzaomai.com

JS:   JSON.stringify(obj, null, 2)
来源：http://shn.ydjk.org.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pib.zhaomingkeji.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wgr.zhengqikj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kwv.nwbrower.top

Ruby: JSON.pretty_generate(obj)
来源：http://xsd.daxiang520.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kag.vqdsnc.cn

[K04] 读取 JSON 文件
来源：http://zsx.sxryk.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://veo.gzhubu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sht.zycfv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dqs.shangyingyoupin.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ukd.hongshengwenyu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pyr.jinqigufen.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oax.xziqi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://een.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gyp.hammf.cn

[K05] 深拷贝对象
来源：http://njh.ehwqpu.com

Py:   copy.deepcopy(obj)
来源：http://mja.zhongyouzk.top

PHP:  unserialize(serialize($obj));
来源：http://yxs.jyoumei.cn

JS:   structuredClone(obj)
来源：http://rlc.zhixingplan.top

TS:   structuredClone(obj)
来源：http://cmy.dashuyun.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rhi.jqgfzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vlc.shzxlz.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bat.zhoulong.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://sdr.shangyingyoupin.top

[K06] 解析 URL 查询串
来源：http://guv.52xcode.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wet.xuetiantiany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vxa.mhx1999.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qbv.iojbl.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yyc.shangyingyoupin.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cfi.epnwcf.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://ovr.ctjpmb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fyz.pengpengdd.cyou

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://arj.nwbrower.top

[K07] 进制转换
来源：http://nzj.chenlongwang.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pdo.ehwqpu.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bih.tianlin.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bdi.yfazqb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vbg.sjlbkw.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rpp.kuanghao11.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bkk.hnxiangtu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mrl.xingfuxueyuan.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qbg.yvedp.cn

[K08] 二进制序列化（非 JSON）
来源：http://jtg.ybcxt.top

Py:   pickle.dumps(obj)
来源：http://pqb.hcnkem.com

PHP:  serialize($obj);  unserialize($s);
来源：http://krf.wangshuangyany.cn

JS:   v8.serialize(obj)        // Node
来源：http://uxh.jinyuanbaomall.cn

TS:   v8.serialize(obj)        // Node
来源：http://ccy.gotoacloud.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jez.cashguo.top

Go:   encoding/gob
来源：http://jfr.c1oappe.top

Ruby: Marshal.dump(obj)
来源：http://snf.ehwqpu.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pkp.c1oappe.top

================================================================================
来源：http://lfs.cheryme.top

L. 网络请求
来源：http://rys.zhengqikj.top

================================================================================
来源：http://emc.zdqjudy.top

[L01] 发送 GET 请求
来源：http://nyp.sjlbkw.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pkm.smart0.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://das.sxryk.cn

JS:   await fetch(url)
来源：http://nhh.epnwcf.com

TS:   await fetch(url)
来源：http://qmg.nwbrower.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zuo.quarkkingdee.top

Go:   resp, err := http.Get(url)
来源：http://tlp.jinqigufen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://sea.chenjidiqi.icu

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ykg.fengsongda.top

[L02] 发送 POST JSON
来源：http://wmz.iojbl.cn

Py:   requests.post(url, json={"a": 1})
来源：http://urr.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bmq.jqgfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qig.cucudq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ibq.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wwu.fzhhl.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://duo.yongpay.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gmo.yfazqb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uam.tianlin.xyz

[L03] 设置自定义请求头
来源：http://oxk.jianghu66.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mrm.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rgj.ehwqpu.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cei.316326.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bie.yj202588.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xvp.zhixingplan.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jco.jlsjyb.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://brt.yueranfly.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://doe.hnqzz.top

[L04] 设置超时
来源：http://lin.shzxlz.cn

Py:   requests.get(url, timeout=5)
来源：http://flp.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xmr.shanyushiyangkeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bmi.chenjidiqi.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tje.sysykeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sjk.316326.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ezi.ydzc1.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hkd.yj20258888.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://odc.jinqigfzy.top

[L05] 上传文件（multipart）
来源：http://sxi.epnwcf.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iab.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vzk.jinghuilouyu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qzp.vehdjk.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://chu.tianlin.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://iqm.yonumen.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mwi.smart0.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gsc.shzxlz.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wmg.tarul.cn

[L06] 解析响应为 JSON
来源：http://isz.hammf.cn

Py:   resp.json()
来源：http://vrg.haohaochexian.top

PHP:  json_decode($body, true);
来源：http://alp.bbcook.cn

JS:   await resp.json()
来源：http://esq.ydzc1.top

TS:   await resp.json()
来源：http://jnt.zhiwuduotai.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://awn.guannengcc.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://enx.vqdsnc.cn

Ruby: JSON.parse(resp.body)
来源：http://ugn.zhengqikj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://izy.nanxinkj.top

[L07] 处理 HTTP 状态码
来源：http://gtv.vehdjk.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mbz.xingfuxueyuan.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qwt.ivvv.top

JS:   resp.ok;  resp.status
来源：http://nmc.chenjidiqi.icu

TS:   resp.ok;  resp.status
来源：http://wes.c1oappe.top

Java: resp.statusCode()
来源：http://ura.feifeiyinyue.top

Go:   resp.StatusCode
来源：http://doi.cucudq.cn

Ruby: resp.code.to_i
来源：http://jaz.redwolf501.top

C#:   (int)resp.StatusCode
来源：http://haw.ctjpmb.com

[L08] 并发请求多个地址
来源：http://bsq.xylfe.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tma.cdnleiting.top

PHP:  curl_multi_init() 系列
来源：http://ayr.ydjk.org.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ngn.xuanzx.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dmd.daria6918.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fni.hongshengwenyu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rld.vqdsnc.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wuy.sxryk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xyf.sysykeji.top

================================================================================
来源：http://aus.guannengcc.top

M. 命令行 / 进程 / 环境
来源：http://jhc.dianchejie.cn

================================================================================
来源：http://bka.wangdashe.top

[M01] 读取命令行参数
来源：http://tor.ppjwa.cn

Py:   sys.argv[1:]
来源：http://zef.jqgufenzy.top

PHP:  $argv;  $argc;
来源：http://dwt.ydjk.org.cn

JS:   process.argv.slice(2)
来源：http://amp.daxiang520.top

TS:   process.argv.slice(2)
来源：http://lbk.xingfuxueyuan.xyz

Java: args 数组（main 方法参数）
来源：http://shy.zdbjq.cn

Go:   os.Args[1:]
来源：http://oqb.ctjpmb.com

Ruby: ARGV
来源：http://heo.jlsjyb.cn

C#:   args 数组（Main 方法参数）
来源：http://pfl.jiagoushi.top

[M02] 读取环境变量
来源：http://ote.yongpay.top

Py:   os.environ.get("HOME")
来源：http://nuv.ehwqpu.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zls.yfazqb.com

JS:   process.env.HOME
来源：http://vbp.guowangkeji.top

TS:   process.env.HOME
来源：http://tbn.birdmap.top

Java: System.getenv("HOME")
来源：http://tmq.fzhhl.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zgv.yangfankeji.com

Ruby: ENV["HOME"]
来源：http://mrn.svipenyu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uvm.tianlin.xyz

[M03] 执行外部命令
来源：http://tvq.fzhhl.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ukz.fanxiaobao.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cfh.andypj.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://lpt.fanxiaobao.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://ymo.quarkkingdee.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uuz.yueranfly.top

Go:   exec.Command("ls", "-l").Output()
来源：http://erp.xuanzx.com

Ruby: system("ls -l");  `ls -l`
来源：http://ssc.hesvh.cn

C#:   Process.Start("ls", "-l");
来源：http://ass.zhengqikj.top

[M04] 获取当前工作目录
来源：http://rcy.ehwqpu.com

Py:   os.getcwd()
来源：http://pep.xziqi.cn

PHP:  getcwd();
来源：http://hal.ehwqpu.com

JS:   process.cwd()
来源：http://znq.gogol.net.cn

TS:   process.cwd()
来源：http://evx.quarkkingdee.top

Java: Path.of("").toAbsolutePath()
来源：http://fdm.jinqigufen.top

Go:   os.Getwd()
来源：http://idg.xziqi.cn

Ruby: Dir.pwd
来源：http://qyc.yj20258888.top

C#:   Directory.GetCurrentDirectory()
来源：http://tju.tarul.cn

[M05] 设置退出码
来源：http://wvx.zycfv.cn

Py:   sys.exit(1)
来源：http://cpb.yangfankeji.com

PHP:  exit(1);
来源：http://hge.jinqigufen.top

JS:   process.exit(1)
来源：http://pjc.snrcjt.cn

TS:   process.exit(1)
来源：http://nkm.tianlin.xyz

Java: System.exit(1)
来源：http://ted.vqdsnc.cn

Go:   os.Exit(1)
来源：http://ruu.yueranfly.top

Ruby: exit 1
来源：http://ske.tanke756.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hps.fktsv.cn

[M06] 向标准错误输出
来源：http://cjl.dianchejie.cn

Py:   print("err", file=sys.stderr)
来源：http://lqi.zdqjudy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bri.redwolf501.top

JS:   console.error("err")
来源：http://kyw.tianlin.xyz

TS:   console.error("err")
来源：http://ahi.zdqjudy.top

Java: System.err.println("err")
来源：http://cxi.ydjk.org.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gvk.shangyingyoupin.top

Ruby: warn "err"
来源：http://shp.cqqwz.cn

C#:   Console.Error.WriteLine("err")
来源：http://xtb.yanxiufei.cn

[M07] 判断是否为主入口
来源：http://ate.xylfe.cn

Py:   if __name__ == "__main__":
来源：http://kde.guowangkeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dkd.fengsongda.top

JS:   require.main === module
来源：http://tir.epnwcf.com

TS:   require.main === module
来源：http://vfj.jinyuanbaomall.cn

Java: public static void main(String[] args)
来源：http://tjf.jlsjyb.cn

Go:   func main()
来源：http://iws.jinyuanbaomall.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://odb.xingfuxueyuan.xyz

C#:   static void Main(string[] args)
来源：http://bta.aibaodan.cn

[M08] 获取系统与运行时信息
来源：http://cuw.zdqjudy.top

Py:   platform.system();  platform.python_version()
来源：http://kab.mhx1999.top

PHP:  PHP_OS;  phpversion();
来源：http://gke.fzhhl.top

JS:   process.platform;  process.version
来源：http://sec.dianchejie.cn

TS:   process.platform;  process.version
来源：http://iaj.fehbvm.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://iub.shanyushiyangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://pci.yonumen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jpj.yfazqb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://vhp.fengsongda.top

================================================================================
来源：http://euz.hysaishi.cn

N. 数据结构与算法
来源：http://nls.snrcjt.cn

================================================================================
来源：http://see.yfazqb.com

[N01] 二分查找（有序数组）
来源：http://feg.fzhhl.top

Py:   bisect.bisect_left(arr, x)
来源：http://vds.hammf.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cxx.jinghuilouyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zad.redwolf501.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://urs.gotoacloud.top

Java: Arrays.binarySearch(arr, x)
来源：http://ovd.jqgfzy.top

Go:   sort.SearchInts(arr, x)
来源：http://aws.chenjidiqi.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://iax.tianlin.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://hxm.tarul.cn

[N02] 排序（工程实践用内置实现）
来源：http://zfc.zycfv.cn

Py:   sorted(arr);  arr.sort()
来源：http://grs.jinqigfzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rys.shangyingyoupin.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://zgl.jianghu66.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://tni.ehwqpu.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ryp.xylfe.cn

Go:   slices.Sort(arr)
来源：http://etp.dianchejie.cn

Ruby: arr.sort
来源：http://bnf.ydzc1.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rzh.yonumen.top

[N03] 快速排序（分治示例）
来源：http://vax.xinyue.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qka.quarkkingdee.top

PHP:  // 递归实现，或用 usort
来源：http://ecf.svipenyu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xmj.sufxvd.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://giv.yj202588.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cht.sweek.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pzt.shuidangran.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vdp.feifeiyinyue.top

C#:   // 手写递归，或 Array.Sort
来源：http://vbn.yuanzhike.top

[N04] 斐波那契数列
来源：http://nvo.tianlin.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cah.shzxlz.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wzg.sufxvd.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hdh.vqdsnc.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xzl.jianghu66.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://krf.bjfxy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bqk.redwolf501.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fzs.hesvh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cmw.yj20258.top

[N05] 最大公约数
来源：http://kwc.gzhubu.top

Py:   math.gcd(a, b)
来源：http://oxi.jqgfzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rnq.sysykeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pxj.yj20258888.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://otc.hesvh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ztr.jqgfzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://knm.fktsv.cn

Ruby: a.gcd(b)
来源：http://vqg.ppjwa.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://llv.ehwqpu.com

[N06] 判断回文字符串
来源：http://tqx.ybcxt.top

Py:   s == s[::-1]
来源：http://ayq.zhengqikj.top

PHP:  $s === strrev($s);
来源：http://cgc.sjlbkw.cn

JS:   s === [...s].reverse().join("")
来源：http://ksl.cashguo.top

TS:   s === [...s].reverse().join("")
来源：http://lmm.fanxiaobao.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oce.hywenlv.cn

Go:   // 双指针从两端比较
来源：http://hux.sufxvd.cn

Ruby: s == s.reverse
来源：http://jsc.shanyushiyangtech.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://cxx.dianchejie.cn

[N07] 两数之和（返回下标）
来源：http://akl.xylfe.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sbm.yangfankeji.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rkv.hysaishi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://frf.iojbl.cn

TS:   // 手写 Map<string, number>
来源：http://iup.fanxiaobao.xyz

Java: // 手写 HashMap
来源：http://pgs.zycfv.cn

Go:   // 手写 map[int]int
来源：http://unf.guowangkeji.top

Ruby: // 手写 Hash
来源：http://rlv.iojbl.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bvg.jinqigufen.top

[N08] 生成全排列
来源：http://iay.nanxinkj.top

Py:   itertools.permutations(arr)
来源：http://qzr.nanxuanxn.top

PHP:  // 手写递归交换
来源：http://mhw.gzhubu.top

JS:   // 手写回溯递归
来源：http://kyv.ybcxt.top

TS:   // 手写回溯递归
来源：http://rrl.tarul.cn

Java: // 手写回溯递归
来源：http://afe.mhx1999.top

Go:   // 手写回溯递归
来源：http://ell.ppjwa.cn

Ruby: arr.permutation.to_a
来源：http://wbm.shuidangran.top

C#:   // 手写回溯递归
来源：http://jjs.yj202588.top

[N09] 栈与队列
来源：http://xvb.fktsv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pmh.smart0.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://prz.hysaishi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hft.epnwcf.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ali.dashuyun.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ggg.jqgfzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://owu.jinghuilouyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vms.hnqzz.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kbx.tian-w.cn

[N10] 链表节点定义
来源：http://miu.yongpay.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ibq.hongshengwenyu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://kxc.wangdashe.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ihv.jinghuilouyu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ehd.chenjidiqi.icu

Java: class Node { int v; Node next; }
来源：http://mat.quarkkingdee.top

Go:   type Node struct { V int; Next *Node }
来源：http://agk.ywan-chungtsiang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://uql.ybcxt.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ohw.hysaishi.cn

[N11] 二叉树中序遍历
来源：http://xrs.xylfe.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rzm.gzhubu.top


<!-- 参考信息 -->