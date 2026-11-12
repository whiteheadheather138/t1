代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ben.xinyue.icu

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oev.zhaomingkeji.xyz

JS:   JSON.stringify(obj)
来源：http://dwq.hammf.cn

TS:   JSON.stringify(obj)
来源：http://cjh.zhijiandao.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jlg.uphjek.com

Go:   json.Marshal(obj)
来源：http://aby.sysykeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://ixx.xuanzx.com

C#:   JsonSerializer.Serialize(obj)
来源：http://jod.dashuyun.cn

[K02] JSON 字符串转对象
来源：http://vgy.sysykeji.top

Py:   json.loads(s)
来源：http://tdk.quarkkingdee.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wau.9152youxi.cn

JS:   JSON.parse(s)
来源：http://wrw.feifeiyinyue.top

TS:   JSON.parse(s)
来源：http://aeo.gotoacloud.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jzz.yongpay.top

Go:   json.Unmarshal(data, &v)
来源：http://dhx.cheryme.top

Ruby: JSON.parse(s)
来源：http://ser.havefunace.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vmp.ydjk.org.cn

[K03] JSON 美化输出（带缩进）
来源：http://wit.gotoacloud.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cea.yanxiufei.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ryg.gotoacloud.top

JS:   JSON.stringify(obj, null, 2)
来源：http://fso.sxryk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://luw.sjlbkw.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://txx.xingfuxueyuan.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hdm.yj20258.top

Ruby: JSON.pretty_generate(obj)
来源：http://isp.shuidangran.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://stj.fengsongda.top

[K04] 读取 JSON 文件
来源：http://bgm.316326.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://amc.ybcxt.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rbc.yj20258.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zez.yueranfly.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oub.hfpthk.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wjn.chenlongwang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qvr.snrcjt.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fxa.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://luj.yj20258888.top

[K05] 深拷贝对象
来源：http://ivw.cashguo.top

Py:   copy.deepcopy(obj)
来源：http://wae.hesvh.cn

PHP:  unserialize(serialize($obj));
来源：http://rvq.cashguo.top

JS:   structuredClone(obj)
来源：http://ofs.jinqigfzy.top

TS:   structuredClone(obj)
来源：http://mza.hammf.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lrz.daria6918.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nwm.guowangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mrh.xingfuxueyuan.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://bnq.pycfn.com

[K06] 解析 URL 查询串
来源：http://ami.yj20258888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uuc.cqqwz.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://amb.mhx1999.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fza.sjlbkw.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gdu.hywenlv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pkb.gaohongyu789.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://hot.sysykeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wpz.smart0.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zpu.vqdsnc.cn

[K07] 进制转换
来源：http://sqk.snrcjt.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wqc.chenlongwang.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zui.yuxming.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ytz.aibaodan.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hnb.nanxinkj.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xxm.havefunace.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zfc.wangdashe.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bve.fzhhl.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iij.feifeiyinyue.top

[K08] 二进制序列化（非 JSON）
来源：http://anm.xuetiantiany.cn

Py:   pickle.dumps(obj)
来源：http://jbm.xuetiantiany.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yfr.zhengqikj.top

JS:   v8.serialize(obj)        // Node
来源：http://vrr.hesvh.cn

TS:   v8.serialize(obj)        // Node
来源：http://dud.gzhubu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bcq.aizwys.cn

Go:   encoding/gob
来源：http://gzu.cqqwz.cn

Ruby: Marshal.dump(obj)
来源：http://vmf.0kj1m.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mse.svipenyu.cn

================================================================================
来源：http://zuv.316326.xyz

L. 网络请求
来源：http://cpw.xinyue.icu

================================================================================
来源：http://ade.yj20258888.top

[L01] 发送 GET 请求
来源：http://jsm.9152youxi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jdw.guowangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qhg.fehbvm.com

JS:   await fetch(url)
来源：http://dbw.meibo888.top

TS:   await fetch(url)
来源：http://kzw.zhengqikj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ock.sxryk.cn

Go:   resp, err := http.Get(url)
来源：http://grs.chenlongwang.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vdo.fehbvm.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vci.snrcjt.cn

[L02] 发送 POST JSON
来源：http://euw.feifeiyinyue.top

Py:   requests.post(url, json={"a": 1})
来源：http://rsc.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tam.gogol.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fol.ydzc1.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ghl.yanxiufei.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pgo.yanxiufei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tgk.hywenlv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://okl.hfpthk.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wjr.fktsv.cn

[L03] 设置自定义请求头
来源：http://fhi.hysaishi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lda.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rtn.ppjwa.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hgi.uphjek.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ygk.gotoacloud.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mas.daxiang520.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cov.9152youxi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sup.yuxming.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jsu.ywan-chungtsiang.top

[L04] 设置超时
来源：http://zul.316326.xyz

Py:   requests.get(url, timeout=5)
来源：http://yfk.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pma.hammf.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mfj.iojbl.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zye.epnwcf.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://soi.guannengcc.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fgy.gotoacloud.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pyk.nanxinkj.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ygl.ehwqpu.com

[L05] 上传文件（multipart）
来源：http://zbp.guannengcc.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xjb.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nud.hfpthk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://grh.snrcjt.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://chl.aizwys.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://efu.yonumen.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dmd.yangfankeji.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lag.xziqi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mka.sysykeji.top

[L06] 解析响应为 JSON
来源：http://izv.yj202588.top

Py:   resp.json()
来源：http://vfq.mhx1999.top

PHP:  json_decode($body, true);
来源：http://day.dianchejie.cn

JS:   await resp.json()
来源：http://bma.wangdashe.top

TS:   await resp.json()
来源：http://lcx.fktsv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hdf.bbcook.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ihq.sweek.top

Ruby: JSON.parse(resp.body)
来源：http://jik.0kj1m.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wwf.nanxuanxn.top

[L07] 处理 HTTP 状态码
来源：http://npd.xziqi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ndh.gzhubu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jro.nanxinkj.top

JS:   resp.ok;  resp.status
来源：http://cud.hammf.cn

TS:   resp.ok;  resp.status
来源：http://ien.jianghu66.top

Java: resp.statusCode()
来源：http://lrn.bjfxy.top

Go:   resp.StatusCode
来源：http://rxt.xziqi.cn

Ruby: resp.code.to_i
来源：http://sdd.zhijiandao.cn

C#:   (int)resp.StatusCode
来源：http://iqx.aizwys.cn

[L08] 并发请求多个地址
来源：http://tvf.birdmap.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dua.fehbvm.com

PHP:  curl_multi_init() 系列
来源：http://twh.snrcjt.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xtn.9152youxi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fau.chenzaomai.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ugu.smart0.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uaf.gaohongyu789.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dwx.chenlongwang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oac.sxryk.cn

================================================================================
来源：http://cli.nanxinkj.top

M. 命令行 / 进程 / 环境
来源：http://tgo.hongshengwenyu.top

================================================================================
来源：http://jdi.sxryk.cn

[M01] 读取命令行参数
来源：http://anp.ctjpmb.com

Py:   sys.argv[1:]
来源：http://phs.yuxming.cn

PHP:  $argv;  $argc;
来源：http://yvf.mhx1999.top

JS:   process.argv.slice(2)
来源：http://jnx.zhoulong.xyz

TS:   process.argv.slice(2)
来源：http://phq.havefunace.top

Java: args 数组（main 方法参数）
来源：http://npw.redwolf501.top

Go:   os.Args[1:]
来源：http://lxn.jinqigufen.top

Ruby: ARGV
来源：http://qhc.sufxvd.cn

C#:   args 数组（Main 方法参数）
来源：http://grv.sxryk.cn

[M02] 读取环境变量
来源：http://wve.fehbvm.com

Py:   os.environ.get("HOME")
来源：http://qhb.cashguo.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zqm.c1oappe.top

JS:   process.env.HOME
来源：http://hnm.jqgfzy.top

TS:   process.env.HOME
来源：http://vhx.yueranfly.top

Java: System.getenv("HOME")
来源：http://vqa.sweek.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tdc.guowangkeji.top

Ruby: ENV["HOME"]
来源：http://xcw.jinyuanbaomall.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hfz.chenjidiqi.icu

[M03] 执行外部命令
来源：http://xxf.yj20258.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ggu.nanxinkj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://skk.smart0.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://lmy.c1oappe.top

TS:   child_process.execSync("ls -l").toString()
来源：http://oqw.yfazqb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cxf.fktsv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gjp.fanxiaobao.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://hxk.havefunace.top

C#:   Process.Start("ls", "-l");
来源：http://lhe.52xcode.cn

[M04] 获取当前工作目录
来源：http://zfv.nanxinkj.top

Py:   os.getcwd()
来源：http://agi.svipenyu.cn

PHP:  getcwd();
来源：http://dxl.hongshengwenyu.top

JS:   process.cwd()
来源：http://grl.ydzc1.top

TS:   process.cwd()
来源：http://ytw.birdmap.top

Java: Path.of("").toAbsolutePath()
来源：http://hio.zdqjudy.top

Go:   os.Getwd()
来源：http://kvg.sufxvd.cn

Ruby: Dir.pwd
来源：http://awa.zhoulong.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://jki.svipenyu.cn

[M05] 设置退出码
来源：http://ncy.c1oappe.top

Py:   sys.exit(1)
来源：http://fnu.daxiang520.top

PHP:  exit(1);
来源：http://djj.9152youxi.cn

JS:   process.exit(1)
来源：http://guj.sweek.top

TS:   process.exit(1)
来源：http://ykg.xinyue.icu

Java: System.exit(1)
来源：http://tyw.zhengqikj.top

Go:   os.Exit(1)
来源：http://lem.sweek.top

Ruby: exit 1
来源：http://qur.xuanzx.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baw.vqdsnc.cn

[M06] 向标准错误输出
来源：http://tee.52xcode.cn

Py:   print("err", file=sys.stderr)
来源：http://qjd.wangshuangyany.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jgv.hywenlv.cn

JS:   console.error("err")
来源：http://hkc.aizwys.cn

TS:   console.error("err")
来源：http://nvm.birdmap.top

Java: System.err.println("err")
来源：http://xnl.zycfv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rdy.sysykeji.top

Ruby: warn "err"
来源：http://ync.feifeiyinyue.top

C#:   Console.Error.WriteLine("err")
来源：http://ffa.jinqigufen.top

[M07] 判断是否为主入口
来源：http://ayi.nwbrower.top

Py:   if __name__ == "__main__":
来源：http://qkf.xuanzx.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mpp.tarul.cn

JS:   require.main === module
来源：http://vbj.haohaochexian.top

TS:   require.main === module
来源：http://jlk.chenjidiqi.icu

Java: public static void main(String[] args)
来源：http://vqz.hnxiangtu.top

Go:   func main()
来源：http://fpr.birdmap.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pfs.quarkkingdee.top

C#:   static void Main(string[] args)
来源：http://upa.birdmap.top

[M08] 获取系统与运行时信息
来源：http://yns.sufxvd.cn

Py:   platform.system();  platform.python_version()
来源：http://zqb.xuetiantiany.cn

PHP:  PHP_OS;  phpversion();
来源：http://hqn.ivvv.top

JS:   process.platform;  process.version
来源：http://fsn.zhoulong.xyz

TS:   process.platform;  process.version
来源：http://rbg.c1oappe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yse.chenzaomai.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://ewm.ydjk.org.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rzm.hywenlv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rnr.jqgfzy.top

================================================================================
来源：http://ohh.yvedp.cn

N. 数据结构与算法
来源：http://rgu.hnxiangtu.top

================================================================================
来源：http://fpx.yanxiufei.cn

[N01] 二分查找（有序数组）
来源：http://gtr.kuanghao11.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ewo.cdnleiting.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wyn.yanxiufei.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fxv.c1oappe.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qqh.xinyue.icu

Java: Arrays.binarySearch(arr, x)
来源：http://jnk.ctjpmb.com

Go:   sort.SearchInts(arr, x)
来源：http://axz.jinghuilouyu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://npf.bbcook.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bjq.pengpengdd.cyou

[N02] 排序（工程实践用内置实现）
来源：http://eoq.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://gwd.yonumen.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ppe.c1oappe.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vnc.c1oappe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://zzk.ywan-chungtsiang.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wdg.bbcook.cn

Go:   slices.Sort(arr)
来源：http://vyg.nwbrower.top

Ruby: arr.sort
来源：http://zje.shzxlz.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://njt.ydzc1.top

[N03] 快速排序（分治示例）
来源：http://qwj.andypj.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jlj.daria6918.cn

PHP:  // 递归实现，或用 usort
来源：http://igc.pycfn.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zsa.shanyushiyangtech.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pui.bbcook.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://aqv.tarul.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uhe.daxiang520.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://axe.hnqzz.top

C#:   // 手写递归，或 Array.Sort
来源：http://cmf.shanyushiyangtech.top

[N04] 斐波那契数列
来源：http://aah.ehwqpu.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yos.xuetiantiany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ges.xuetiantiany.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fmr.fzhhl.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://icb.vehdjk.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hyn.hfpthk.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://aqf.havefunace.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hii.redwolf501.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yef.guannengcc.top

[N05] 最大公约数
来源：http://rrk.jianghu66.top

Py:   math.gcd(a, b)
来源：http://yep.guowangkeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://och.dashuyun.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gfw.wangdashe.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zfb.meibo888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ybn.shuidangran.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kyt.fanxiaobao.xyz

Ruby: a.gcd(b)
来源：http://nnr.hnqzz.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://iyu.hfpthk.cn

[N06] 判断回文字符串
来源：http://ftk.vehdjk.com

Py:   s == s[::-1]
来源：http://adp.jinqigfzy.top

PHP:  $s === strrev($s);
来源：http://kbh.yanxiufei.cn

JS:   s === [...s].reverse().join("")
来源：http://klg.quarkkingdee.top

TS:   s === [...s].reverse().join("")
来源：http://mai.yfazqb.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hxf.fktsv.cn

Go:   // 双指针从两端比较
来源：http://zzq.snrcjt.cn

Ruby: s == s.reverse
来源：http://huk.mhx1999.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xot.nanxinkj.top

[N07] 两数之和（返回下标）
来源：http://lua.0kj1m.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oby.sxryk.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yim.shzxlz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yfd.fanxiaobao.xyz

TS:   // 手写 Map<string, number>
来源：http://wwr.bjfxy.top

Java: // 手写 HashMap
来源：http://bzo.ehwqpu.com

Go:   // 手写 map[int]int
来源：http://uva.hammf.cn

Ruby: // 手写 Hash
来源：http://mls.shzxlz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nbg.gotoacloud.top

[N08] 生成全排列
来源：http://cpe.yanxiufei.cn

Py:   itertools.permutations(arr)
来源：http://pjz.yj20258888.top

PHP:  // 手写递归交换
来源：http://zbx.cdnleiting.top

JS:   // 手写回溯递归
来源：http://qne.yanxiufei.cn

TS:   // 手写回溯递归
来源：http://lbo.ydjk.org.cn

Java: // 手写回溯递归
来源：http://uqg.yonumen.top

Go:   // 手写回溯递归
来源：http://vbd.gzhubu.top

Ruby: arr.permutation.to_a
来源：http://slb.ctjpmb.com

C#:   // 手写回溯递归
来源：http://zda.chenlongwang.top

[N09] 栈与队列
来源：http://siq.shzxlz.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vzp.chenzaomai.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rvk.dashuyun.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lmv.zhengqikj.top


<!-- 参考信息 -->