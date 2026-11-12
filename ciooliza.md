代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://dsu.zhengqikj.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ger.shanyushiyangtech.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://trj.daria6918.cn

Ruby: d1 < d2;  d1 == d2
来源：http://dve.fktsv.cn

C#:   d1 < d2;  d1 == d2
来源：http://ghn.redwolf501.top

[J08] 提取年月日与星期
来源：http://aco.cdnleiting.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iou.ydjk.org.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gys.gaohongyu789.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://faa.pycfn.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rms.hnxiangtu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oii.xinyue.icu

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tlf.fehbvm.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://omm.52xcode.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sid.fzhhl.top

[J09] 时区处理
来源：http://cjj.yvedp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cfp.haohaochexian.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hra.yueranfly.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sdn.yangfankeji.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vyv.52xcode.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fxk.sjlbkw.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nij.jinqigfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://tob.yj202588.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qul.iojbl.cn

[J10] 取今天 / 本月第一天
来源：http://oql.hammf.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nsx.zhiwuduotai.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://juh.iojbl.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tdq.gotoacloud.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rwp.zhengqikj.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ozg.hfpthk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jjq.hcnkem.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ttz.shangyingyoupin.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://olh.pengpengdd.cyou

================================================================================
来源：http://lbl.zhaomingkeji.xyz

K. JSON 与序列化
来源：http://miu.havefunace.top

================================================================================
来源：http://joi.jinghuilouyu.cn

[K01] 对象转 JSON 字符串
来源：http://kgu.gogol.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xnu.hammf.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xiy.gaohongyu789.top

JS:   JSON.stringify(obj)
来源：http://ncg.sufxvd.cn

TS:   JSON.stringify(obj)
来源：http://ujt.chenzaomai.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hmr.nwbrower.top

Go:   json.Marshal(obj)
来源：http://ofc.snrcjt.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xev.iojbl.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wkk.tian-w.cn

[K02] JSON 字符串转对象
来源：http://kcr.sweek.top

Py:   json.loads(s)
来源：http://sut.hfpthk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://std.sjlbkw.cn

JS:   JSON.parse(s)
来源：http://tpa.svipenyu.cn

TS:   JSON.parse(s)
来源：http://oql.zhoulong.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mdy.shuidangran.top

Go:   json.Unmarshal(data, &v)
来源：http://lmx.nwbrower.top

Ruby: JSON.parse(s)
来源：http://qtu.epnwcf.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://che.yanxiufei.cn

[K03] JSON 美化输出（带缩进）
来源：http://rcb.chenjidiqi.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kpz.yfazqb.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wcc.hywenlv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zen.daxiang520.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mlh.0kj1m.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tda.ppjwa.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://det.52xcode.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rqb.bbcook.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gok.cashguo.top

[K04] 读取 JSON 文件
来源：http://ute.jianghu66.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kfo.jinqigufen.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nnf.tanke756.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hjb.yj202588.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gal.sufxvd.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cwr.dashuyun.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uqc.52xcode.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rsh.shanyushiyangtech.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kca.jinqigfzy.top

[K05] 深拷贝对象
来源：http://ndk.svipenyu.cn

Py:   copy.deepcopy(obj)
来源：http://fuu.fktsv.cn

PHP:  unserialize(serialize($obj));
来源：http://nro.zdqjudy.top

JS:   structuredClone(obj)
来源：http://ucb.yueranfly.top

TS:   structuredClone(obj)
来源：http://lkw.aibaodan.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ili.sjlbkw.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xlc.aizwys.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nkd.jlsjyb.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bcp.iojbl.cn

[K06] 解析 URL 查询串
来源：http://atn.hongshengwenyu.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://moi.ydjk.org.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cad.zhongyouzk.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mdm.jlsjyb.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bfq.tianlin.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uxk.aibaodan.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://euv.jqgufenzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rmu.chenjidiqi.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://oke.yvedp.cn

[K07] 进制转换
来源：http://ojs.cdnleiting.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fff.gogol.net.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rth.ybcxt.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qph.hongshengwenyu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://igh.ctjpmb.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pxi.jqgufenzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uig.wangshuangyany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kii.pycfn.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zdw.xinyue.icu

[K08] 二进制序列化（非 JSON）
来源：http://snl.tanke756.top

Py:   pickle.dumps(obj)
来源：http://jyb.vqdsnc.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://eaj.pengpengdd.cyou

JS:   v8.serialize(obj)        // Node
来源：http://cjo.yuanzhike.top

TS:   v8.serialize(obj)        // Node
来源：http://deu.cheryme.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vlt.uphjek.com

Go:   encoding/gob
来源：http://cba.hfpthk.cn

Ruby: Marshal.dump(obj)
来源：http://bpj.xinyue.icu

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qes.dashuyun.cn

================================================================================
来源：http://lzf.hysaishi.cn

L. 网络请求
来源：http://kpb.sufxvd.cn

================================================================================
来源：http://xln.jyoumei.cn

[L01] 发送 GET 请求
来源：http://okv.hammf.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xhe.yanxiufei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bxv.fehbvm.com

JS:   await fetch(url)
来源：http://zyi.birdmap.top

TS:   await fetch(url)
来源：http://acq.cheryme.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fnx.jinghuilouyu.cn

Go:   resp, err := http.Get(url)
来源：http://oxu.shuidangran.top

Ruby: Net::HTTP.get(URI(url))
来源：http://fcu.ydjk.org.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kli.yfazqb.com

[L02] 发送 POST JSON
来源：http://grd.zhijiandao.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zvc.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lqm.cashguo.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tsf.haohaochexian.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uto.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lxc.hammf.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wsw.sweek.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wai.kuanghao11.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ufj.c1oappe.top

[L03] 设置自定义请求头
来源：http://cep.hcnkem.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mwe.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bpl.xziqi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fku.chenzaomai.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gti.316326.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://guc.nwbrower.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jcp.zhoulong.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ebi.ivvv.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://agw.xziqi.cn

[L04] 设置超时
来源：http://bpd.wangshuangyany.cn

Py:   requests.get(url, timeout=5)
来源：http://llw.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nnl.jinghuilouyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sij.nanxinkj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xtr.haohaochexian.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jvx.epnwcf.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uze.hysaishi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uvm.zdbjq.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hfs.guannengcc.top

[L05] 上传文件（multipart）
来源：http://uza.pycfn.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://aoe.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sqp.tianlin.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cwb.yongpay.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eke.chenlongwang.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fkz.vehdjk.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qwo.iojbl.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ldi.zycfv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bky.wangshuangyany.cn

[L06] 解析响应为 JSON
来源：http://dnc.yueranfly.top

Py:   resp.json()
来源：http://pif.vqdsnc.cn

PHP:  json_decode($body, true);
来源：http://euz.xziqi.cn

JS:   await resp.json()
来源：http://kxy.nanxinkj.top

TS:   await resp.json()
来源：http://pkz.fanxiaobao.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://azs.fktsv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yjy.hfpthk.cn

Ruby: JSON.parse(resp.body)
来源：http://kmi.jinqigufen.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wwy.nanxinkj.top

[L07] 处理 HTTP 状态码
来源：http://ool.meibo888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vwh.feifeiyinyue.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ppx.xinyue.icu

JS:   resp.ok;  resp.status
来源：http://ryd.0kj1m.cn

TS:   resp.ok;  resp.status
来源：http://uxv.daxiang520.top

Java: resp.statusCode()
来源：http://clm.chenlongwang.top

Go:   resp.StatusCode
来源：http://zps.yfazqb.com

Ruby: resp.code.to_i
来源：http://vww.smart0.xyz

C#:   (int)resp.StatusCode
来源：http://lth.meibo888.top

[L08] 并发请求多个地址
来源：http://bmo.hywenlv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mff.yfazqb.com

PHP:  curl_multi_init() 系列
来源：http://ptz.zycfv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xav.sufxvd.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rxd.meibo888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dnt.zhengqikj.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yyy.fzhhl.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rxl.hcnkem.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nzh.xziqi.cn

================================================================================
来源：http://mgr.nwbrower.top

M. 命令行 / 进程 / 环境
来源：http://ttz.chenjidiqi.icu

================================================================================
来源：http://rfq.xuetiantiany.cn

[M01] 读取命令行参数
来源：http://plb.bjfxy.top

Py:   sys.argv[1:]
来源：http://slu.tian-w.cn

PHP:  $argv;  $argc;
来源：http://mya.cashguo.top

JS:   process.argv.slice(2)
来源：http://ygc.pengpengdd.cyou

TS:   process.argv.slice(2)
来源：http://acj.yj20258888.top

Java: args 数组（main 方法参数）
来源：http://bad.yongpay.top

Go:   os.Args[1:]
来源：http://yxl.xuanzx.com

Ruby: ARGV
来源：http://syg.epnwcf.com

C#:   args 数组（Main 方法参数）
来源：http://mlc.52xcode.cn

[M02] 读取环境变量
来源：http://xau.vehdjk.com

Py:   os.environ.get("HOME")
来源：http://lpi.sufxvd.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jpp.sxryk.cn

JS:   process.env.HOME
来源：http://msn.jqgfzy.top

TS:   process.env.HOME
来源：http://dce.kuanghao11.cn

Java: System.getenv("HOME")
来源：http://ldx.havefunace.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jrd.yfazqb.com

Ruby: ENV["HOME"]
来源：http://qbn.xingfuxueyuan.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://htm.wangshuangyany.cn

[M03] 执行外部命令
来源：http://cno.zdbjq.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tph.yuxming.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dfv.feifeiyinyue.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jll.birdmap.top

TS:   child_process.execSync("ls -l").toString()
来源：http://tcu.zhaomingkeji.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zma.yj20258888.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ons.guannengcc.top

Ruby: system("ls -l");  `ls -l`
来源：http://uvh.quarkkingdee.top

C#:   Process.Start("ls", "-l");
来源：http://tpx.ivvv.top

[M04] 获取当前工作目录
来源：http://aeh.yueranfly.top

Py:   os.getcwd()
来源：http://llz.tian-w.cn

PHP:  getcwd();
来源：http://vlr.tanke756.top

JS:   process.cwd()
来源：http://lhi.tarul.cn

TS:   process.cwd()
来源：http://jdr.ywan-chungtsiang.top

Java: Path.of("").toAbsolutePath()
来源：http://xej.xinyue.icu

Go:   os.Getwd()
来源：http://hmp.tarul.cn

Ruby: Dir.pwd
来源：http://qme.wangshuangyany.cn

C#:   Directory.GetCurrentDirectory()
来源：http://guc.gogol.net.cn

[M05] 设置退出码
来源：http://rar.jiagoushi.top

Py:   sys.exit(1)
来源：http://gir.gaohongyu789.top

PHP:  exit(1);
来源：http://otk.jlsjyb.cn

JS:   process.exit(1)
来源：http://ctu.zhiwuduotai.top

TS:   process.exit(1)
来源：http://zez.epnwcf.com

Java: System.exit(1)
来源：http://efn.tian-w.cn

Go:   os.Exit(1)
来源：http://yat.chenzaomai.com

Ruby: exit 1
来源：http://sgx.jyoumei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xdm.snrcjt.cn

[M06] 向标准错误输出
来源：http://chy.pycfn.com

Py:   print("err", file=sys.stderr)
来源：http://gjj.hnqzz.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mbf.zhixingplan.top

JS:   console.error("err")
来源：http://bxn.cucudq.cn

TS:   console.error("err")
来源：http://jsn.yvedp.cn

Java: System.err.println("err")
来源：http://aqr.jinqigufen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pbf.sweek.top

Ruby: warn "err"
来源：http://xmo.cqqwz.cn

C#:   Console.Error.WriteLine("err")
来源：http://gwz.snrcjt.cn

[M07] 判断是否为主入口
来源：http://dte.wangshuangyany.cn

Py:   if __name__ == "__main__":
来源：http://bzv.hammf.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mpg.yangfankeji.com

JS:   require.main === module
来源：http://rpd.sxryk.cn

TS:   require.main === module
来源：http://dav.birdmap.top

Java: public static void main(String[] args)
来源：http://xhy.jlsjyb.cn

Go:   func main()
来源：http://jwm.cdnleiting.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://grb.yuxming.cn

C#:   static void Main(string[] args)
来源：http://psj.vehdjk.com

[M08] 获取系统与运行时信息
来源：http://lxb.quarkkingdee.top

Py:   platform.system();  platform.python_version()
来源：http://qxt.shanyushiyangtech.top

PHP:  PHP_OS;  phpversion();
来源：http://ckz.ybcxt.top

JS:   process.platform;  process.version
来源：http://zzd.yvedp.cn

TS:   process.platform;  process.version
来源：http://bxy.cdnleiting.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ygu.hongshengwenyu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xcq.sysykeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vok.ctjpmb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://ade.chenzaomai.com

================================================================================
来源：http://snx.fengsongda.top

N. 数据结构与算法
来源：http://vte.gotoacloud.top

================================================================================
来源：http://why.hnxiangtu.top

[N01] 二分查找（有序数组）
来源：http://hxf.52xcode.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dsx.xuetiantiany.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eis.birdmap.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lhe.daria6918.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jqk.hysaishi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lwj.0kj1m.cn

Go:   sort.SearchInts(arr, x)
来源：http://wfz.cqqwz.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://oup.hnxiangtu.top

C#:   Array.BinarySearch(arr, x)
来源：http://yyw.shzxlz.cn

[N02] 排序（工程实践用内置实现）
来源：http://ksu.gotoacloud.top

Py:   sorted(arr);  arr.sort()
来源：http://ykn.jyoumei.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rnb.yj20258.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://eed.yfazqb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://ckx.hongshengwenyu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ptx.vehdjk.com

Go:   slices.Sort(arr)
来源：http://opy.shzxlz.cn

Ruby: arr.sort
来源：http://qeb.svipenyu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vdm.jinqigufen.top

[N03] 快速排序（分治示例）
来源：http://pcp.yangfankeji.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hts.xuanzx.com

PHP:  // 递归实现，或用 usort
来源：http://wfs.hesvh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hhn.zhiwuduotai.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ula.c1oappe.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pzj.dashuyun.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xiw.hammf.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uhf.tianlin.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://rrp.gaohongyu789.top

[N04] 斐波那契数列
来源：http://qzb.haohaochexian.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mbi.pengpengdd.cyou

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xyq.yuxming.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zyc.chenlongwang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aco.0kj1m.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lot.quarkkingdee.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lfv.kuanghao11.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ygu.zhixingplan.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dyc.vehdjk.com

[N05] 最大公约数
来源：http://wij.jyoumei.cn

Py:   math.gcd(a, b)
来源：http://xdf.iojbl.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fpn.ydjk.org.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xri.zhiwuduotai.top


<!-- 参考信息 -->