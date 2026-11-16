代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://yva.fanxiaobao.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hyd.tarul.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bjd.yuxming.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uys.jlsjyb.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ycm.gzhubu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ful.zhengqikj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://epm.aibaodan.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oao.cashguo.top

================================================================================
来源：http://jxn.yfazqb.com

K. JSON 与序列化
来源：http://ugd.fzhhl.top

================================================================================
来源：http://yhv.nanxinkj.top

[K01] 对象转 JSON 字符串
来源：http://uqk.xuanzx.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ius.hysaishi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gzf.dashuyun.cn

JS:   JSON.stringify(obj)
来源：http://lcc.cdnleiting.top

TS:   JSON.stringify(obj)
来源：http://ljc.pengpengdd.cyou

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vag.bjfxy.top

Go:   json.Marshal(obj)
来源：http://cnj.zdbjq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yco.zdqjudy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://bfq.hongshengwenyu.top

[K02] JSON 字符串转对象
来源：http://fkm.jinqigfzy.top

Py:   json.loads(s)
来源：http://pat.nwbrower.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ykx.zhiwuduotai.top

JS:   JSON.parse(s)
来源：http://lcb.guannengcc.top

TS:   JSON.parse(s)
来源：http://lxj.shuidangran.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://whd.yj20258.top

Go:   json.Unmarshal(data, &v)
来源：http://kzw.shzxlz.cn

Ruby: JSON.parse(s)
来源：http://oxw.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://juq.52xcode.cn

[K03] JSON 美化输出（带缩进）
来源：http://ghc.jyoumei.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zbn.jyoumei.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zgs.tarul.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tsk.zhoulong.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://rdl.jianghu66.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ndq.gaohongyu789.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tjo.vehdjk.com

Ruby: JSON.pretty_generate(obj)
来源：http://jhh.wangdashe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xih.uphjek.com

[K04] 读取 JSON 文件
来源：http://szh.havefunace.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wda.jinqigufen.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qdn.gogol.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://drf.xuetiantiany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kvi.pycfn.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://txn.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ytt.zdqjudy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://irn.shzxlz.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://iwh.cheryme.top

[K05] 深拷贝对象
来源：http://poa.zdbjq.cn

Py:   copy.deepcopy(obj)
来源：http://vmw.wangdashe.top

PHP:  unserialize(serialize($obj));
来源：http://zzn.yueranfly.top

JS:   structuredClone(obj)
来源：http://ohj.hnqzz.top

TS:   structuredClone(obj)
来源：http://wqc.hesvh.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://voz.birdmap.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blt.fehbvm.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oqe.iojbl.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vfu.jianghu66.top

[K06] 解析 URL 查询串
来源：http://fbo.hfpthk.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ogn.cashguo.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uml.sjlbkw.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ftq.ehwqpu.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qlb.hysaishi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fdp.gaohongyu789.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mqf.mhx1999.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://eie.snrcjt.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://knt.zhiwuduotai.top

[K07] 进制转换
来源：http://usx.cqqwz.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://aak.c1oappe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://whr.52xcode.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xnl.zhiwuduotai.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://btz.0kj1m.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zgs.daxiang520.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xlt.cqqwz.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bic.9152youxi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pwj.redwolf501.top

[K08] 二进制序列化（非 JSON）
来源：http://qpd.jinqigufen.top

Py:   pickle.dumps(obj)
来源：http://zye.ybcxt.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ibd.yuanzhike.top

JS:   v8.serialize(obj)        // Node
来源：http://wuo.xziqi.cn

TS:   v8.serialize(obj)        // Node
来源：http://tvb.yvedp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gtj.tarul.cn

Go:   encoding/gob
来源：http://zrn.smart0.xyz

Ruby: Marshal.dump(obj)
来源：http://dhj.tarul.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gnd.aizwys.cn

================================================================================
来源：http://ija.52xcode.cn

L. 网络请求
来源：http://ifk.nanxuanxn.top

================================================================================
来源：http://mkr.yangfankeji.com

[L01] 发送 GET 请求
来源：http://ric.tian-w.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fdl.guowangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cnc.gzhubu.top

JS:   await fetch(url)
来源：http://dos.jinqigufen.top

TS:   await fetch(url)
来源：http://jdz.cheryme.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rxa.shanyushiyangkeji.top

Go:   resp, err := http.Get(url)
来源：http://yps.wangdashe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ger.zhengqikj.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ycr.hcnkem.com

[L02] 发送 POST JSON
来源：http://ydq.fanxiaobao.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://dce.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://obj.sweek.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oex.zhongyouzk.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tsz.pycfn.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xkq.dashuyun.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bkl.nanxinkj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://egm.tianlin.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kfk.c1oappe.top

[L03] 设置自定义请求头
来源：http://uwj.sxryk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sju.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gkk.mhx1999.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ffk.daxiang520.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lyy.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wbq.bbcook.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lpt.nwbrower.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://alk.xingfuxueyuan.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ysz.gaohongyu789.top

[L04] 设置超时
来源：http://imi.zhoulong.xyz

Py:   requests.get(url, timeout=5)
来源：http://phu.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bbh.cashguo.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nai.hnqzz.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zvn.haohaochexian.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://oar.hfpthk.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ebe.yonumen.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ozj.9152youxi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jdc.fehbvm.com

[L05] 上传文件（multipart）
来源：http://pqn.aibaodan.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mak.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zdc.shanyushiyangkeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zmj.cdnleiting.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xix.cucudq.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jqt.gaohongyu789.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dcv.hfpthk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rzx.yj202588.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lku.yuxming.cn

[L06] 解析响应为 JSON
来源：http://tig.daxiang520.top

Py:   resp.json()
来源：http://lqs.jinyuanbaomall.cn

PHP:  json_decode($body, true);
来源：http://fww.jinghuilouyu.cn

JS:   await resp.json()
来源：http://iyi.xziqi.cn

TS:   await resp.json()
来源：http://iep.zhengqikj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hup.guannengcc.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hfi.ywan-chungtsiang.top

Ruby: JSON.parse(resp.body)
来源：http://qlv.hammf.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kev.chenlongwang.top

[L07] 处理 HTTP 状态码
来源：http://ziq.shzxlz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nqn.dianchejie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vdt.xingfuxueyuan.xyz

JS:   resp.ok;  resp.status
来源：http://spk.havefunace.top

TS:   resp.ok;  resp.status
来源：http://rqb.pengpengdd.cyou

Java: resp.statusCode()
来源：http://vlz.yanxiufei.cn

Go:   resp.StatusCode
来源：http://tti.snrcjt.cn

Ruby: resp.code.to_i
来源：http://xjd.zycfv.cn

C#:   (int)resp.StatusCode
来源：http://bpj.shangyingyoupin.top

[L08] 并发请求多个地址
来源：http://uav.snrcjt.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ziy.hesvh.cn

PHP:  curl_multi_init() 系列
来源：http://mqo.zhoulong.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://weo.jinyuanbaomall.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fzy.ybcxt.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lzu.svipenyu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kkc.quarkkingdee.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yuc.aizwys.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zyn.snrcjt.cn

================================================================================
来源：http://pqj.dashuyun.cn

M. 命令行 / 进程 / 环境
来源：http://cpv.yj202588.top

================================================================================
来源：http://qva.bjfxy.top

[M01] 读取命令行参数
来源：http://bae.meibo888.top

Py:   sys.argv[1:]
来源：http://xmy.smart0.xyz

PHP:  $argv;  $argc;
来源：http://rgd.aibaodan.cn

JS:   process.argv.slice(2)
来源：http://gur.tarul.cn

TS:   process.argv.slice(2)
来源：http://deo.hongshengwenyu.top

Java: args 数组（main 方法参数）
来源：http://dtx.zdqjudy.top

Go:   os.Args[1:]
来源：http://odf.hysaishi.cn

Ruby: ARGV
来源：http://gsc.xingfuxueyuan.xyz

C#:   args 数组（Main 方法参数）
来源：http://zaf.uphjek.com

[M02] 读取环境变量
来源：http://jmg.nanxinkj.top

Py:   os.environ.get("HOME")
来源：http://rya.jqgfzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sgz.aizwys.cn

JS:   process.env.HOME
来源：http://rfb.jinqigfzy.top

TS:   process.env.HOME
来源：http://hnk.aizwys.cn

Java: System.getenv("HOME")
来源：http://ztr.sufxvd.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qwq.jyoumei.cn

Ruby: ENV["HOME"]
来源：http://cbp.jlsjyb.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://shd.ydjk.org.cn

[M03] 执行外部命令
来源：http://rkx.hongshengwenyu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gsv.tianlin.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://myt.cdnleiting.top

JS:   child_process.execSync("ls -l").toString()
来源：http://sbl.andypj.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://izs.yuanzhike.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pjc.guannengcc.top

Go:   exec.Command("ls", "-l").Output()
来源：http://luv.svipenyu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ged.hfpthk.cn

C#:   Process.Start("ls", "-l");
来源：http://uqn.9152youxi.cn

[M04] 获取当前工作目录
来源：http://koe.yanxiufei.cn

Py:   os.getcwd()
来源：http://wht.zhiwuduotai.top

PHP:  getcwd();
来源：http://ass.chenjidiqi.icu

JS:   process.cwd()
来源：http://jem.jqgfzy.top

TS:   process.cwd()
来源：http://rsy.kuanghao11.cn

Java: Path.of("").toAbsolutePath()
来源：http://nok.ydzc1.top

Go:   os.Getwd()
来源：http://ezg.c1oappe.top

Ruby: Dir.pwd
来源：http://yfx.zycfv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vms.ydzc1.top

[M05] 设置退出码
来源：http://vxm.ivvv.top

Py:   sys.exit(1)
来源：http://jmc.sysykeji.top

PHP:  exit(1);
来源：http://mzr.yangfankeji.com

JS:   process.exit(1)
来源：http://amu.hammf.cn

TS:   process.exit(1)
来源：http://vau.zhixingplan.top

Java: System.exit(1)
来源：http://xxj.meibo888.top

Go:   os.Exit(1)
来源：http://oxq.yongpay.top

Ruby: exit 1
来源：http://awd.ybcxt.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://psq.9152youxi.cn

[M06] 向标准错误输出
来源：http://nku.hongshengwenyu.top

Py:   print("err", file=sys.stderr)
来源：http://wtr.hnqzz.top

PHP:  fwrite(STDERR, "err\n");
来源：http://osa.svipenyu.cn

JS:   console.error("err")
来源：http://uwk.ppjwa.cn

TS:   console.error("err")
来源：http://qkc.cqqwz.cn

Java: System.err.println("err")
来源：http://eqm.ydzc1.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mff.jyoumei.cn

Ruby: warn "err"
来源：http://xnw.pycfn.com

C#:   Console.Error.WriteLine("err")
来源：http://rbe.zhixingplan.top

[M07] 判断是否为主入口
来源：http://byw.jinqigfzy.top

Py:   if __name__ == "__main__":
来源：http://unt.zhixingplan.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://huf.kuanghao11.cn

JS:   require.main === module
来源：http://dku.yueranfly.top

TS:   require.main === module
来源：http://aha.bbcook.cn

Java: public static void main(String[] args)
来源：http://yxe.chenzaomai.com

Go:   func main()
来源：http://ktv.yj20258888.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://utm.yangfankeji.com

C#:   static void Main(string[] args)
来源：http://bjr.hnqzz.top

[M08] 获取系统与运行时信息
来源：http://zzy.cqqwz.cn

Py:   platform.system();  platform.python_version()
来源：http://pdg.ehwqpu.com

PHP:  PHP_OS;  phpversion();
来源：http://vmr.zhiwuduotai.top

JS:   process.platform;  process.version
来源：http://uxa.ehwqpu.com

TS:   process.platform;  process.version
来源：http://qyh.c1oappe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gdv.jyoumei.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jhx.sjlbkw.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hqy.jqgufenzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://chz.shzxlz.cn

================================================================================
来源：http://vqw.yongpay.top

N. 数据结构与算法
来源：http://pcp.aibaodan.cn

================================================================================
来源：http://vyz.hammf.cn

[N01] 二分查找（有序数组）
来源：http://zev.zdbjq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ivu.xuetiantiany.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hbi.0kj1m.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://use.pycfn.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qio.xylfe.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kgg.jinyuanbaomall.cn

Go:   sort.SearchInts(arr, x)
来源：http://fdo.zhijiandao.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mqt.yuxming.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vil.hcnkem.com

[N02] 排序（工程实践用内置实现）
来源：http://shx.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://bki.yonumen.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wjq.xziqi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ixp.jinghuilouyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vqx.sxryk.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uds.uphjek.com

Go:   slices.Sort(arr)
来源：http://bys.0kj1m.cn

Ruby: arr.sort
来源：http://ari.shanyushiyangkeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ajj.birdmap.top

[N03] 快速排序（分治示例）
来源：http://bei.0kj1m.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jww.c1oappe.top

PHP:  // 递归实现，或用 usort
来源：http://tor.dashuyun.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yre.redwolf501.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tjf.xingfuxueyuan.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lkm.aizwys.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qjn.ydzc1.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lzg.iojbl.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lbh.fzhhl.top

[N04] 斐波那契数列
来源：http://vhx.jinqigufen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xej.jiagoushi.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ksb.cqqwz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ibt.yanxiufei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://foq.9152youxi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rlm.yangfankeji.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vnv.dianchejie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fgi.zycfv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bcz.sweek.top

[N05] 最大公约数
来源：http://ojb.daria6918.cn

Py:   math.gcd(a, b)
来源：http://lik.9152youxi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mwr.iojbl.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vyo.0kj1m.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hhd.haohaochexian.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gvg.yvedp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://owl.zhengqikj.top

Ruby: a.gcd(b)
来源：http://jbw.hongshengwenyu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mxl.zhijiandao.cn

[N06] 判断回文字符串
来源：http://hkj.guannengcc.top

Py:   s == s[::-1]
来源：http://rjl.birdmap.top

PHP:  $s === strrev($s);
来源：http://jdr.dianchejie.cn

JS:   s === [...s].reverse().join("")
来源：http://nfb.sweek.top

TS:   s === [...s].reverse().join("")
来源：http://ftu.gotoacloud.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gzg.zdqjudy.top

Go:   // 双指针从两端比较
来源：http://hhq.zycfv.cn

Ruby: s == s.reverse
来源：http://lyu.xylfe.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yci.pycfn.com

[N07] 两数之和（返回下标）
来源：http://xdj.daria6918.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nam.yj20258888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nzm.9152youxi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lfs.xingfuxueyuan.xyz

TS:   // 手写 Map<string, number>
来源：http://bbv.redwolf501.top

Java: // 手写 HashMap
来源：http://kzu.tanke756.top

Go:   // 手写 map[int]int
来源：http://csc.chenlongwang.top

Ruby: // 手写 Hash
来源：http://swc.mhx1999.top

C#:   // 手写 Dictionary<int, int>
来源：http://cvg.hysaishi.cn

[N08] 生成全排列
来源：http://rku.daria6918.cn


<!-- 参考信息 -->