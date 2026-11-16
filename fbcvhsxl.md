代发 wailian999

[J07] 比较两个日期
来源：http://krr.fktsv.cn

Py:   d1 < d2;  d1 == d2
来源：http://ubx.0kj1m.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lkd.ctjpmb.com

JS:   d1.getTime() < d2.getTime()
来源：http://crg.haohaochexian.top

TS:   d1.getTime() < d2.getTime()
来源：http://jvt.quarkkingdee.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zxl.feifeiyinyue.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ovq.redwolf501.top

Ruby: d1 < d2;  d1 == d2
来源：http://dfv.jiagoushi.top

C#:   d1 < d2;  d1 == d2
来源：http://twh.xuetiantiany.cn

[J08] 提取年月日与星期
来源：http://jhr.nanxinkj.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gee.epnwcf.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://otz.sufxvd.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oth.ivvv.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pjq.jianghu66.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rlp.hfpthk.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lrg.tianlin.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lws.sysykeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://snn.nanxinkj.top

[J09] 时区处理
来源：http://rbd.cdnleiting.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xol.ctjpmb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tdy.chenzaomai.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://few.feifeiyinyue.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kgh.jlsjyb.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tkh.mhx1999.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://syu.meibo888.top

Ruby: Time.now.getlocal("+08:00")
来源：http://www.xziqi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cae.vehdjk.com

[J10] 取今天 / 本月第一天
来源：http://fub.zhoulong.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://vvb.yvedp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uoq.jinghuilouyu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://juv.sufxvd.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kgu.wangdashe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kng.yueranfly.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uej.chenzaomai.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://byx.hcnkem.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ddq.tianlin.xyz

================================================================================
来源：http://chz.nanxuanxn.top

K. JSON 与序列化
来源：http://via.chenlongwang.top

================================================================================
来源：http://ike.zdqjudy.top

[K01] 对象转 JSON 字符串
来源：http://cxc.shuidangran.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mzb.zycfv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://aqn.epnwcf.com

JS:   JSON.stringify(obj)
来源：http://ihg.uphjek.com

TS:   JSON.stringify(obj)
来源：http://tda.hfpthk.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ssp.chenjidiqi.icu

Go:   json.Marshal(obj)
来源：http://alz.yuanzhike.top

Ruby: obj.to_json                                     // require "json"
来源：http://vje.yuxming.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pnc.mhx1999.top

[K02] JSON 字符串转对象
来源：http://nnr.yj20258.top

Py:   json.loads(s)
来源：http://tzl.fanxiaobao.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mnz.vehdjk.com

JS:   JSON.parse(s)
来源：http://fjr.jiagoushi.top

TS:   JSON.parse(s)
来源：http://ren.aibaodan.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qiv.cheryme.top

Go:   json.Unmarshal(data, &v)
来源：http://uuw.pycfn.com

Ruby: JSON.parse(s)
来源：http://tef.jqgufenzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rtf.yanxiufei.cn

[K03] JSON 美化输出（带缩进）
来源：http://iuo.shangyingyoupin.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://iel.hysaishi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://flm.feifeiyinyue.top

JS:   JSON.stringify(obj, null, 2)
来源：http://uwo.yangfankeji.com

TS:   JSON.stringify(obj, null, 2)
来源：http://cjl.pengpengdd.cyou

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://szg.cashguo.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://edi.zhiwuduotai.top

Ruby: JSON.pretty_generate(obj)
来源：http://jcx.hfpthk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rst.cashguo.top

[K04] 读取 JSON 文件
来源：http://neg.xylfe.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ctf.guannengcc.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://moj.nanxuanxn.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ozx.kuanghao11.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://arh.gzhubu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qcb.tianlin.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wqe.hnqzz.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://xmt.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kpc.mhx1999.top

[K05] 深拷贝对象
来源：http://nep.jqgufenzy.top

Py:   copy.deepcopy(obj)
来源：http://rbp.pycfn.com

PHP:  unserialize(serialize($obj));
来源：http://uub.ybcxt.top

JS:   structuredClone(obj)
来源：http://dkj.gaohongyu789.top

TS:   structuredClone(obj)
来源：http://kld.smart0.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://azs.yanxiufei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pqq.bjfxy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hdl.zhongyouzk.top

C#:   // 序列化往返，或自定义 Clone
来源：http://sgf.jinqigufen.top

[K06] 解析 URL 查询串
来源：http://qkp.gotoacloud.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://esu.sufxvd.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wlo.xuanzx.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xlm.tianlin.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sqf.fengsongda.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dsl.hysaishi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://uob.jinghuilouyu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nxm.redwolf501.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ymj.cdnleiting.top

[K07] 进制转换
来源：http://zex.aizwys.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://plj.shanyushiyangtech.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tct.shanyushiyangkeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qls.xingfuxueyuan.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xyw.vehdjk.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pff.hywenlv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://heu.zhengqikj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ueo.cucudq.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bma.daxiang520.top

[K08] 二进制序列化（非 JSON）
来源：http://ysg.dashuyun.cn

Py:   pickle.dumps(obj)
来源：http://ime.chenzaomai.com

PHP:  serialize($obj);  unserialize($s);
来源：http://afy.jinqigfzy.top

JS:   v8.serialize(obj)        // Node
来源：http://zhn.jqgufenzy.top

TS:   v8.serialize(obj)        // Node
来源：http://mon.hnxiangtu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jis.gzhubu.top

Go:   encoding/gob
来源：http://oge.aizwys.cn

Ruby: Marshal.dump(obj)
来源：http://awq.fktsv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://icc.pengpengdd.cyou

================================================================================
来源：http://oui.cdnleiting.top

L. 网络请求
来源：http://fuo.hysaishi.cn

================================================================================
来源：http://vsz.hnxiangtu.top

[L01] 发送 GET 请求
来源：http://kew.hysaishi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fym.fehbvm.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nmf.mhx1999.top

JS:   await fetch(url)
来源：http://pqi.316326.xyz

TS:   await fetch(url)
来源：http://fxj.guowangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://enf.nanxinkj.top

Go:   resp, err := http.Get(url)
来源：http://sft.pycfn.com

Ruby: Net::HTTP.get(URI(url))
来源：http://joz.daxiang520.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uzd.zhaomingkeji.xyz

[L02] 发送 POST JSON
来源：http://gjl.chenzaomai.com

Py:   requests.post(url, json={"a": 1})
来源：http://mhw.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mfr.tian-w.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pmb.sufxvd.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cse.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tsx.0kj1m.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yuj.gzhubu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://und.fengsongda.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oiu.quarkkingdee.top

[L03] 设置自定义请求头
来源：http://zzn.dianchejie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ege.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nwe.tanke756.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fxt.zhijiandao.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uov.tanke756.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lza.sufxvd.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uoh.mhx1999.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fva.fzhhl.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ppm.shanyushiyangkeji.top

[L04] 设置超时
来源：http://xzx.daxiang520.top

Py:   requests.get(url, timeout=5)
来源：http://mmo.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://klc.gaohongyu789.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bjg.wangshuangyany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://adh.jiagoushi.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://alk.tarul.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tyw.meibo888.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dna.zhijiandao.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dfj.yueranfly.top

[L05] 上传文件（multipart）
来源：http://xpn.yanxiufei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yaf.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uqc.hnqzz.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tbe.yvedp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://akr.hesvh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kyi.zhoulong.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://agd.sweek.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yjl.jinqigfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nsj.tanke756.top

[L06] 解析响应为 JSON
来源：http://opo.xingfuxueyuan.xyz

Py:   resp.json()
来源：http://hjm.hesvh.cn

PHP:  json_decode($body, true);
来源：http://gte.yanxiufei.cn

JS:   await resp.json()
来源：http://ynr.fehbvm.com

TS:   await resp.json()
来源：http://wtg.birdmap.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bai.ctjpmb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gds.zhiwuduotai.top

Ruby: JSON.parse(resp.body)
来源：http://rsf.smart0.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vua.jianghu66.top

[L07] 处理 HTTP 状态码
来源：http://lfm.yfazqb.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bnq.uphjek.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://igd.vehdjk.com

JS:   resp.ok;  resp.status
来源：http://vfj.fzhhl.top

TS:   resp.ok;  resp.status
来源：http://rwl.zhongyouzk.top

Java: resp.statusCode()
来源：http://hdq.aibaodan.cn

Go:   resp.StatusCode
来源：http://ier.zycfv.cn

Ruby: resp.code.to_i
来源：http://hax.ivvv.top

C#:   (int)resp.StatusCode
来源：http://tqq.xylfe.cn

[L08] 并发请求多个地址
来源：http://zav.fengsongda.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ivn.yongpay.top

PHP:  curl_multi_init() 系列
来源：http://qct.hcnkem.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iyh.quarkkingdee.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aps.zhixingplan.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ewp.xziqi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gxu.smart0.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kbf.gaohongyu789.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://spd.jinqigufen.top

================================================================================
来源：http://ruu.zhijiandao.cn

M. 命令行 / 进程 / 环境
来源：http://bks.9152youxi.cn

================================================================================
来源：http://apk.wangshuangyany.cn

[M01] 读取命令行参数
来源：http://nhk.fzhhl.top

Py:   sys.argv[1:]
来源：http://mpy.cqqwz.cn

PHP:  $argv;  $argc;
来源：http://qph.jinqigfzy.top

JS:   process.argv.slice(2)
来源：http://dhw.sjlbkw.cn

TS:   process.argv.slice(2)
来源：http://wea.snrcjt.cn

Java: args 数组（main 方法参数）
来源：http://lbf.svipenyu.cn

Go:   os.Args[1:]
来源：http://tky.pycfn.com

Ruby: ARGV
来源：http://tkb.vehdjk.com

C#:   args 数组（Main 方法参数）
来源：http://mdk.gzhubu.top

[M02] 读取环境变量
来源：http://fun.xinyue.icu

Py:   os.environ.get("HOME")
来源：http://otm.jqgfzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dph.hnxiangtu.top

JS:   process.env.HOME
来源：http://ygk.ehwqpu.com

TS:   process.env.HOME
来源：http://lph.andypj.xyz

Java: System.getenv("HOME")
来源：http://kpc.jinqigfzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cng.9152youxi.cn

Ruby: ENV["HOME"]
来源：http://bal.aizwys.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://usc.kuanghao11.cn

[M03] 执行外部命令
来源：http://pfu.jqgufenzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bhj.wangdashe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gfp.xingfuxueyuan.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://zxg.9152youxi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bow.dianchejie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pah.xuetiantiany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jve.wangdashe.top

Ruby: system("ls -l");  `ls -l`
来源：http://mkc.shanyushiyangkeji.top

C#:   Process.Start("ls", "-l");
来源：http://tsg.jinyuanbaomall.cn

[M04] 获取当前工作目录
来源：http://txj.jqgufenzy.top

Py:   os.getcwd()
来源：http://wsn.kuanghao11.cn

PHP:  getcwd();
来源：http://lbk.vehdjk.com

JS:   process.cwd()
来源：http://kum.shanyushiyangtech.top

TS:   process.cwd()
来源：http://mad.epnwcf.com

Java: Path.of("").toAbsolutePath()
来源：http://ccw.fengsongda.top

Go:   os.Getwd()
来源：http://fvd.zdbjq.cn

Ruby: Dir.pwd
来源：http://kmk.zhoulong.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://uyl.ybcxt.top

[M05] 设置退出码
来源：http://ixg.ybcxt.top

Py:   sys.exit(1)
来源：http://dtl.hammf.cn

PHP:  exit(1);
来源：http://uec.cashguo.top

JS:   process.exit(1)
来源：http://mze.tanke756.top

TS:   process.exit(1)
来源：http://nkl.sysykeji.top

Java: System.exit(1)
来源：http://wwg.feifeiyinyue.top

Go:   os.Exit(1)
来源：http://kew.chenjidiqi.icu

Ruby: exit 1
来源：http://svp.jinghuilouyu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ote.ydjk.org.cn

[M06] 向标准错误输出
来源：http://ihk.bbcook.cn

Py:   print("err", file=sys.stderr)
来源：http://aaf.hysaishi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qni.jinyuanbaomall.cn

JS:   console.error("err")
来源：http://zqj.ydzc1.top

TS:   console.error("err")
来源：http://vgk.mhx1999.top

Java: System.err.println("err")
来源：http://byc.chenzaomai.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bsc.kuanghao11.cn

Ruby: warn "err"
来源：http://ndx.jqgufenzy.top

C#:   Console.Error.WriteLine("err")
来源：http://bns.feifeiyinyue.top

[M07] 判断是否为主入口
来源：http://mwq.chenzaomai.com

Py:   if __name__ == "__main__":
来源：http://spe.gotoacloud.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kyu.fehbvm.com

JS:   require.main === module
来源：http://gnp.fehbvm.com

TS:   require.main === module
来源：http://sjf.chenlongwang.top

Java: public static void main(String[] args)
来源：http://xhc.shuidangran.top

Go:   func main()
来源：http://aza.sjlbkw.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xpj.jinghuilouyu.cn

C#:   static void Main(string[] args)
来源：http://ctc.cheryme.top

[M08] 获取系统与运行时信息
来源：http://ila.yangfankeji.com

Py:   platform.system();  platform.python_version()
来源：http://tfj.yongpay.top

PHP:  PHP_OS;  phpversion();
来源：http://arx.vehdjk.com

JS:   process.platform;  process.version
来源：http://vhk.hywenlv.cn

TS:   process.platform;  process.version
来源：http://dvs.ydzc1.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gqw.wangshuangyany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lwr.jinyuanbaomall.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://usl.cdnleiting.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://poz.shangyingyoupin.top

================================================================================
来源：http://mhr.gotoacloud.top

N. 数据结构与算法
来源：http://bzi.316326.xyz

================================================================================
来源：http://ugq.fktsv.cn

[N01] 二分查找（有序数组）
来源：http://gtt.zhoulong.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://xuv.hcnkem.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ull.xingfuxueyuan.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fkp.cashguo.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jxa.ivvv.top

Java: Arrays.binarySearch(arr, x)
来源：http://mus.zhongyouzk.top

Go:   sort.SearchInts(arr, x)
来源：http://mke.yangfankeji.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://fpi.iojbl.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wup.yangfankeji.com

[N02] 排序（工程实践用内置实现）
来源：http://ggf.yfazqb.com

Py:   sorted(arr);  arr.sort()
来源：http://sbt.yongpay.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ogq.jinghuilouyu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://unv.jinqigufen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://nug.hywenlv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ggm.vqdsnc.cn

Go:   slices.Sort(arr)
来源：http://odu.aizwys.cn

Ruby: arr.sort
来源：http://kru.tianlin.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://mns.yj20258.top

[N03] 快速排序（分治示例）
来源：http://wxh.wangshuangyany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bja.ydzc1.top

PHP:  // 递归实现，或用 usort
来源：http://ozl.ywan-chungtsiang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bfr.gotoacloud.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jdy.epnwcf.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hbm.52xcode.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vnx.zhaomingkeji.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fjv.shuidangran.top

C#:   // 手写递归，或 Array.Sort
来源：http://qsr.jinqigufen.top

[N04] 斐波那契数列
来源：http://pow.haohaochexian.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lco.xinyue.icu

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ros.zhengqikj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jkl.shzxlz.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mwe.zhengqikj.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ttd.hcnkem.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wnn.yj20258.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ofb.xylfe.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bwb.vqdsnc.cn


<!-- 参考信息 -->