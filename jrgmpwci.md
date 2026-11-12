代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ehe.tian-w.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jjt.zhixingplan.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gwl.fengsongda.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ehs.jinqigfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bjz.aibaodan.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wzy.jinghuilouyu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ufx.ywan-chungtsiang.top

[J10] 取今天 / 本月第一天
来源：http://ozp.xuetiantiany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tnb.chenlongwang.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zdj.yangfankeji.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ifs.jinqigufen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lsn.shangyingyoupin.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cck.wangdashe.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ina.yj20258.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wfc.sjlbkw.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qwr.yuanzhike.top

================================================================================
来源：http://lna.c1oappe.top

K. JSON 与序列化
来源：http://skn.tianlin.xyz

================================================================================
来源：http://the.vqdsnc.cn

[K01] 对象转 JSON 字符串
来源：http://jcj.guannengcc.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nls.hesvh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://eut.yuxming.cn

JS:   JSON.stringify(obj)
来源：http://qke.cucudq.cn

TS:   JSON.stringify(obj)
来源：http://ngw.epnwcf.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rui.hnxiangtu.top

Go:   json.Marshal(obj)
来源：http://mxh.yj202588.top

Ruby: obj.to_json                                     // require "json"
来源：http://tsy.gogol.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zta.sufxvd.cn

[K02] JSON 字符串转对象
来源：http://ljj.yj20258.top

Py:   json.loads(s)
来源：http://zxu.svipenyu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zsw.zhaomingkeji.xyz

JS:   JSON.parse(s)
来源：http://jpf.cashguo.top

TS:   JSON.parse(s)
来源：http://ngb.smart0.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nbd.chenjidiqi.icu

Go:   json.Unmarshal(data, &v)
来源：http://ivg.gzhubu.top

Ruby: JSON.parse(s)
来源：http://epj.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sel.guannengcc.top

[K03] JSON 美化输出（带缩进）
来源：http://pio.jianghu66.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://geh.dashuyun.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gyh.feifeiyinyue.top

JS:   JSON.stringify(obj, null, 2)
来源：http://mlo.kuanghao11.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lgv.svipenyu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://aes.c1oappe.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mib.cdnleiting.top

Ruby: JSON.pretty_generate(obj)
来源：http://ndu.jianghu66.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bbi.hywenlv.cn

[K04] 读取 JSON 文件
来源：http://eza.52xcode.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mac.redwolf501.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mmd.zhijiandao.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vko.sjlbkw.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dni.ehwqpu.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fpv.shuidangran.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dhc.havefunace.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://reu.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ghy.hysaishi.cn

[K05] 深拷贝对象
来源：http://nbb.9152youxi.cn

Py:   copy.deepcopy(obj)
来源：http://mvm.uphjek.com

PHP:  unserialize(serialize($obj));
来源：http://rlg.xziqi.cn

JS:   structuredClone(obj)
来源：http://gqf.shanyushiyangkeji.top

TS:   structuredClone(obj)
来源：http://hfe.jianghu66.top

Java: // 手写拷贝构造，或序列化往返
来源：http://zkw.yuanzhike.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tep.pengpengdd.cyou

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cpn.shangyingyoupin.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jdr.yongpay.top

[K06] 解析 URL 查询串
来源：http://rwm.tianlin.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://phg.cdnleiting.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qob.cucudq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xqd.shangyingyoupin.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hyx.zhengqikj.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://noe.uphjek.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://gqw.ppjwa.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://otq.ivvv.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wce.guowangkeji.top

[K07] 进制转换
来源：http://mtr.snrcjt.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rao.jinghuilouyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jqq.gzhubu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ynk.yvedp.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tkb.zdbjq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xei.iojbl.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rhf.hnxiangtu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mso.svipenyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qhb.aizwys.cn

[K08] 二进制序列化（非 JSON）
来源：http://drq.jlsjyb.cn

Py:   pickle.dumps(obj)
来源：http://yyr.redwolf501.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qcg.ybcxt.top

JS:   v8.serialize(obj)        // Node
来源：http://ezs.tarul.cn

TS:   v8.serialize(obj)        // Node
来源：http://owu.jinqigufen.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ton.aibaodan.cn

Go:   encoding/gob
来源：http://jau.dianchejie.cn

Ruby: Marshal.dump(obj)
来源：http://pea.aizwys.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tcm.dashuyun.cn

================================================================================
来源：http://btj.xziqi.cn

L. 网络请求
来源：http://ydo.tianlin.xyz

================================================================================
来源：http://odd.tanke756.top

[L01] 发送 GET 请求
来源：http://qye.vehdjk.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xko.daxiang520.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://afv.daria6918.cn

JS:   await fetch(url)
来源：http://mzc.zhengqikj.top

TS:   await fetch(url)
来源：http://vlj.chenlongwang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kgd.gogol.net.cn

Go:   resp, err := http.Get(url)
来源：http://bao.pengpengdd.cyou

Ruby: Net::HTTP.get(URI(url))
来源：http://huy.cucudq.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dqe.gzhubu.top

[L02] 发送 POST JSON
来源：http://syy.cdnleiting.top

Py:   requests.post(url, json={"a": 1})
来源：http://bif.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fwh.dashuyun.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://byf.iojbl.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cru.zhoulong.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://reo.yuanzhike.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://one.zhoulong.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zsm.316326.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ntj.fzhhl.top

[L03] 设置自定义请求头
来源：http://icg.gotoacloud.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vui.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://iof.yueranfly.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mmn.cucudq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tlh.nwbrower.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ghf.9152youxi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xkz.wangdashe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://igr.daxiang520.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://smj.52xcode.cn

[L04] 设置超时
来源：http://hhs.jiagoushi.top

Py:   requests.get(url, timeout=5)
来源：http://wrk.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qbu.gogol.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xnm.tianlin.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lvv.haohaochexian.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ail.yvedp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://itm.bbcook.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://epm.vqdsnc.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zos.yongpay.top

[L05] 上传文件（multipart）
来源：http://vpg.sweek.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bze.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://klu.gotoacloud.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nvo.daxiang520.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qwi.yfazqb.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rdl.aibaodan.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://omr.cqqwz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ayx.jlsjyb.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hua.iojbl.cn

[L06] 解析响应为 JSON
来源：http://pyd.daria6918.cn

Py:   resp.json()
来源：http://jdk.c1oappe.top

PHP:  json_decode($body, true);
来源：http://cub.hcnkem.com

JS:   await resp.json()
来源：http://dku.chenlongwang.top

TS:   await resp.json()
来源：http://pwv.jqgfzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lyn.sxryk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bav.9152youxi.cn

Ruby: JSON.parse(resp.body)
来源：http://ltz.nwbrower.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://knt.haohaochexian.top

[L07] 处理 HTTP 状态码
来源：http://mll.feifeiyinyue.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jhk.bbcook.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yxu.hcnkem.com

JS:   resp.ok;  resp.status
来源：http://jbc.gogol.net.cn

TS:   resp.ok;  resp.status
来源：http://jxe.cucudq.cn

Java: resp.statusCode()
来源：http://wkt.yj20258888.top

Go:   resp.StatusCode
来源：http://gxd.nwbrower.top

Ruby: resp.code.to_i
来源：http://pjt.sxryk.cn

C#:   (int)resp.StatusCode
来源：http://iop.zhengqikj.top

[L08] 并发请求多个地址
来源：http://wai.52xcode.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cpm.vqdsnc.cn

PHP:  curl_multi_init() 系列
来源：http://lzr.pycfn.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://auq.jinqigfzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bub.hywenlv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ppy.bjfxy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eoi.havefunace.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vst.yj20258.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uss.ppjwa.cn

================================================================================
来源：http://jhm.jqgufenzy.top

M. 命令行 / 进程 / 环境
来源：http://esw.wangshuangyany.cn

================================================================================
来源：http://xgb.316326.xyz

[M01] 读取命令行参数
来源：http://fsj.birdmap.top

Py:   sys.argv[1:]
来源：http://wun.fktsv.cn

PHP:  $argv;  $argc;
来源：http://kjn.jinghuilouyu.cn

JS:   process.argv.slice(2)
来源：http://poo.zhongyouzk.top

TS:   process.argv.slice(2)
来源：http://guz.jiagoushi.top

Java: args 数组（main 方法参数）
来源：http://hso.gaohongyu789.top

Go:   os.Args[1:]
来源：http://fnm.daria6918.cn

Ruby: ARGV
来源：http://tuv.jinqigfzy.top

C#:   args 数组（Main 方法参数）
来源：http://ljr.yuxming.cn

[M02] 读取环境变量
来源：http://oyd.jlsjyb.cn

Py:   os.environ.get("HOME")
来源：http://gin.zycfv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rly.yj202588.top

JS:   process.env.HOME
来源：http://bga.gogol.net.cn

TS:   process.env.HOME
来源：http://juo.xziqi.cn

Java: System.getenv("HOME")
来源：http://vmw.jinghuilouyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dmy.jqgfzy.top

Ruby: ENV["HOME"]
来源：http://tko.nanxinkj.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ylh.shanyushiyangtech.top

[M03] 执行外部命令
来源：http://slr.chenzaomai.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zpb.cheryme.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zvn.tian-w.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tas.chenzaomai.com

TS:   child_process.execSync("ls -l").toString()
来源：http://vly.ctjpmb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qkj.52xcode.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rsn.vehdjk.com

Ruby: system("ls -l");  `ls -l`
来源：http://ewk.jqgufenzy.top

C#:   Process.Start("ls", "-l");
来源：http://nre.chenjidiqi.icu

[M04] 获取当前工作目录
来源：http://xnl.tarul.cn

Py:   os.getcwd()
来源：http://itp.ywan-chungtsiang.top

PHP:  getcwd();
来源：http://flb.bbcook.cn

JS:   process.cwd()
来源：http://rmb.sjlbkw.cn

TS:   process.cwd()
来源：http://vxc.jianghu66.top

Java: Path.of("").toAbsolutePath()
来源：http://azb.shanyushiyangkeji.top

Go:   os.Getwd()
来源：http://plo.jinqigufen.top

Ruby: Dir.pwd
来源：http://qsf.jinqigfzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://nue.chenjidiqi.icu

[M05] 设置退出码
来源：http://qeb.hongshengwenyu.top

Py:   sys.exit(1)
来源：http://xgw.nanxuanxn.top

PHP:  exit(1);
来源：http://ryw.zhixingplan.top

JS:   process.exit(1)
来源：http://dhh.fanxiaobao.xyz

TS:   process.exit(1)
来源：http://mmb.zhaomingkeji.xyz

Java: System.exit(1)
来源：http://xgc.chenzaomai.com

Go:   os.Exit(1)
来源：http://ffj.fzhhl.top

Ruby: exit 1
来源：http://ufg.dianchejie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fyg.smart0.xyz

[M06] 向标准错误输出
来源：http://dhb.xingfuxueyuan.xyz

Py:   print("err", file=sys.stderr)
来源：http://ulo.ydzc1.top

PHP:  fwrite(STDERR, "err\n");
来源：http://trs.wangshuangyany.cn

JS:   console.error("err")
来源：http://qoa.zhongyouzk.top

TS:   console.error("err")
来源：http://ubd.fktsv.cn

Java: System.err.println("err")
来源：http://vvx.tarul.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dst.quarkkingdee.top

Ruby: warn "err"
来源：http://xrq.gogol.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://szc.chenjidiqi.icu

[M07] 判断是否为主入口
来源：http://cvh.jinghuilouyu.cn

Py:   if __name__ == "__main__":
来源：http://ukq.316326.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://alu.zhongyouzk.top

JS:   require.main === module
来源：http://xcn.hesvh.cn

TS:   require.main === module
来源：http://vbp.yj20258888.top

Java: public static void main(String[] args)
来源：http://wlx.nwbrower.top

Go:   func main()
来源：http://jsu.bbcook.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gag.yangfankeji.com

C#:   static void Main(string[] args)
来源：http://clu.fengsongda.top

[M08] 获取系统与运行时信息
来源：http://gpp.guannengcc.top

Py:   platform.system();  platform.python_version()
来源：http://sqo.xziqi.cn

PHP:  PHP_OS;  phpversion();
来源：http://dur.cashguo.top

JS:   process.platform;  process.version
来源：http://jhw.pengpengdd.cyou

TS:   process.platform;  process.version
来源：http://fct.ydjk.org.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xid.jqgufenzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ipq.jlsjyb.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hkv.jianghu66.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://pyq.shzxlz.cn

================================================================================
来源：http://xej.hfpthk.cn

N. 数据结构与算法
来源：http://eve.tarul.cn

================================================================================
来源：http://cts.0kj1m.cn

[N01] 二分查找（有序数组）
来源：http://han.wangshuangyany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hib.dashuyun.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bse.ywan-chungtsiang.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://urr.yj202588.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hyb.yonumen.top

Java: Arrays.binarySearch(arr, x)
来源：http://btu.zhoulong.xyz

Go:   sort.SearchInts(arr, x)
来源：http://snb.sxryk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pgn.fzhhl.top

C#:   Array.BinarySearch(arr, x)
来源：http://cnl.jqgufenzy.top

[N02] 排序（工程实践用内置实现）
来源：http://qsk.xinyue.icu

Py:   sorted(arr);  arr.sort()
来源：http://tnx.zdqjudy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cuh.sxryk.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fpx.ivvv.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://yzr.gzhubu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zzo.xuanzx.com

Go:   slices.Sort(arr)
来源：http://thu.sweek.top

Ruby: arr.sort
来源：http://oqx.pengpengdd.cyou

C#:   Array.Sort(arr);  list.Sort()
来源：http://ito.ctjpmb.com

[N03] 快速排序（分治示例）
来源：http://lbj.jyoumei.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://aub.shanyushiyangkeji.top

PHP:  // 递归实现，或用 usort
来源：http://qwg.ywan-chungtsiang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://erq.hnxiangtu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rmw.aibaodan.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wsd.yangfankeji.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rtc.jinqigfzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qwu.tian-w.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dmf.cashguo.top

[N04] 斐波那契数列
来源：http://ekq.nwbrower.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://teg.cheryme.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hfc.0kj1m.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kml.snrcjt.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://meb.c1oappe.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jjp.tanke756.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lem.jqgfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vrd.gogol.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qxu.jyoumei.cn

[N05] 最大公约数
来源：http://zmu.pycfn.com

Py:   math.gcd(a, b)
来源：http://tbg.gogol.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ebc.gotoacloud.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ogr.tanke756.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bpg.ppjwa.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fet.jyoumei.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://got.snrcjt.cn

Ruby: a.gcd(b)
来源：http://mmd.hongshengwenyu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://drr.hcnkem.com

[N06] 判断回文字符串
来源：http://jgs.cucudq.cn

Py:   s == s[::-1]
来源：http://xrn.yuxming.cn

PHP:  $s === strrev($s);
来源：http://ius.jinghuilouyu.cn

JS:   s === [...s].reverse().join("")
来源：http://geu.jinqigfzy.top

TS:   s === [...s].reverse().join("")
来源：http://xbk.316326.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wce.sufxvd.cn

Go:   // 双指针从两端比较
来源：http://the.haohaochexian.top

Ruby: s == s.reverse
来源：http://yla.aibaodan.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://juc.daxiang520.top

[N07] 两数之和（返回下标）
来源：http://ytt.gaohongyu789.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://njy.hysaishi.cn


<!-- 参考信息 -->