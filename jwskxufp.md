代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://dsp.tian-w.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wsw.tian-w.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gvu.zhaomingkeji.xyz

Java: LocalDate.now().plusDays(7)
来源：http://bqy.zhixingplan.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iia.hesvh.cn

Ruby: Time.now + 7 * 86400
来源：http://wsx.yuanzhike.top

C#:   DateTime.Now.AddDays(7)
来源：http://pvu.hesvh.cn

[J06] 计算两时间之差
来源：http://gdi.havefunace.top

Py:   (end - start).total_seconds()
来源：http://pnp.jyoumei.cn

PHP:  $end->diff($start)->days;
来源：http://zcu.jqgfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yjv.jqgufenzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pgk.nanxuanxn.top

Java: Duration.between(start, end).toSeconds()
来源：http://yqf.nanxinkj.top

Go:   end.Sub(start).Hours()
来源：http://dfx.hfpthk.cn

Ruby: end - start                 # 返回秒数
来源：http://ytd.chenjidiqi.icu

C#:   (end - start).TotalSeconds
来源：http://rzx.chenjidiqi.icu

[J07] 比较两个日期
来源：http://rcq.ehwqpu.com

Py:   d1 < d2;  d1 == d2
来源：http://nip.ybcxt.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ksg.zhongyouzk.top

JS:   d1.getTime() < d2.getTime()
来源：http://ohp.redwolf501.top

TS:   d1.getTime() < d2.getTime()
来源：http://ufh.ydzc1.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hul.gotoacloud.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://plh.zhaomingkeji.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://gqf.sysykeji.top

C#:   d1 < d2;  d1 == d2
来源：http://jcf.316326.xyz

[J08] 提取年月日与星期
来源：http://bsk.chenjidiqi.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kao.ybcxt.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bgz.fzhhl.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://prx.fanxiaobao.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hzg.cheryme.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://puz.xuetiantiany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vlo.hnqzz.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cmi.nwbrower.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hje.jinqigufen.top

[J09] 时区处理
来源：http://yzw.nwbrower.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://anl.yuanzhike.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://djp.fengsongda.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xat.jiagoushi.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cqq.shanyushiyangkeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bhw.sxryk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wkc.hesvh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gpi.fengsongda.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://szl.ivvv.top

[J10] 取今天 / 本月第一天
来源：http://ixn.cucudq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ggo.ywan-chungtsiang.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ioo.zhaomingkeji.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wxm.meibo888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zii.yongpay.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nfe.xylfe.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dsj.nanxuanxn.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zpt.tarul.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://swh.pengpengdd.cyou

================================================================================
来源：http://aob.yvedp.cn

K. JSON 与序列化
来源：http://zri.hnqzz.top

================================================================================
来源：http://igb.zhengqikj.top

[K01] 对象转 JSON 字符串
来源：http://wli.tanke756.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.pycfn.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uik.gotoacloud.top

JS:   JSON.stringify(obj)
来源：http://fxs.zdbjq.cn

TS:   JSON.stringify(obj)
来源：http://pfv.jiagoushi.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kef.fktsv.cn

Go:   json.Marshal(obj)
来源：http://dai.meibo888.top

Ruby: obj.to_json                                     // require "json"
来源：http://omy.shzxlz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zzi.sysykeji.top

[K02] JSON 字符串转对象
来源：http://qmo.hnxiangtu.top

Py:   json.loads(s)
来源：http://sjg.shzxlz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tkx.guannengcc.top

JS:   JSON.parse(s)
来源：http://jjs.smart0.xyz

TS:   JSON.parse(s)
来源：http://ems.hysaishi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lpb.xuetiantiany.cn

Go:   json.Unmarshal(data, &v)
来源：http://pxq.epnwcf.com

Ruby: JSON.parse(s)
来源：http://kzv.gaohongyu789.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://saz.xuanzx.com

[K03] JSON 美化输出（带缩进）
来源：http://tcw.52xcode.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nop.gogol.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://uld.jinqigfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://pgi.sysykeji.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xej.aizwys.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://swz.fktsv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fvx.52xcode.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wbv.zhoulong.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://but.yj202588.top

[K04] 读取 JSON 文件
来源：http://clr.shuidangran.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tbj.hfpthk.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dic.birdmap.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fyh.meibo888.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://esg.zycfv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://byf.redwolf501.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mxh.fehbvm.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://lxz.shanyushiyangtech.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fgw.0kj1m.cn

[K05] 深拷贝对象
来源：http://ldu.yongpay.top

Py:   copy.deepcopy(obj)
来源：http://zkz.birdmap.top

PHP:  unserialize(serialize($obj));
来源：http://tom.bjfxy.top

JS:   structuredClone(obj)
来源：http://klt.sufxvd.cn

TS:   structuredClone(obj)
来源：http://jnl.aizwys.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sxt.jiagoushi.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tfg.havefunace.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xod.hnqzz.top

C#:   // 序列化往返，或自定义 Clone
来源：http://gqj.hesvh.cn

[K06] 解析 URL 查询串
来源：http://cuc.zhaomingkeji.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jfr.zdbjq.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://elw.yongpay.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ofg.sxryk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fvh.52xcode.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yam.redwolf501.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://vvn.yueranfly.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uee.sweek.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tbd.yvedp.cn

[K07] 进制转换
来源：http://jcl.chenzaomai.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mpy.dianchejie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jir.birdmap.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lom.chenlongwang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lzg.fktsv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wjq.tian-w.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://koq.gogol.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wuc.svipenyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zjp.yfazqb.com

[K08] 二进制序列化（非 JSON）
来源：http://usf.yangfankeji.com

Py:   pickle.dumps(obj)
来源：http://bqm.0kj1m.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://uvz.zhiwuduotai.top

JS:   v8.serialize(obj)        // Node
来源：http://wnh.zhixingplan.top

TS:   v8.serialize(obj)        // Node
来源：http://xly.xuanzx.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pyj.pycfn.com

Go:   encoding/gob
来源：http://seh.daria6918.cn

Ruby: Marshal.dump(obj)
来源：http://gkt.yj202588.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lpw.yvedp.cn

================================================================================
来源：http://wbc.yangfankeji.com

L. 网络请求
来源：http://xou.gaohongyu789.top

================================================================================
来源：http://qfn.yongpay.top

[L01] 发送 GET 请求
来源：http://elh.fanxiaobao.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ccj.jinghuilouyu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://avb.fktsv.cn

JS:   await fetch(url)
来源：http://ixb.fktsv.cn

TS:   await fetch(url)
来源：http://lkv.yfazqb.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wyt.hesvh.cn

Go:   resp, err := http.Get(url)
来源：http://bov.yvedp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yjx.cqqwz.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ypl.hywenlv.cn

[L02] 发送 POST JSON
来源：http://kip.meibo888.top

Py:   requests.post(url, json={"a": 1})
来源：http://nwy.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://faa.yfazqb.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://emc.redwolf501.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://clr.hesvh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://erg.zdqjudy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://doe.tian-w.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zou.mhx1999.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ola.hesvh.cn

[L03] 设置自定义请求头
来源：http://xff.zhijiandao.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zuu.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fvp.zhongyouzk.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kxa.ctjpmb.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hdn.sjlbkw.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wsj.quarkkingdee.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ghz.uphjek.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ejl.quarkkingdee.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pfi.xylfe.cn

[L04] 设置超时
来源：http://siw.0kj1m.cn

Py:   requests.get(url, timeout=5)
来源：http://een.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xkn.fengsongda.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://faq.cqqwz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://irc.sufxvd.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tra.52xcode.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dml.snrcjt.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://szw.9152youxi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hoz.52xcode.cn

[L05] 上传文件（multipart）
来源：http://etl.cdnleiting.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ktr.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://iwp.snrcjt.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zmj.nanxinkj.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mow.tian-w.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dav.yj20258888.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uai.316326.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ger.tarul.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qza.yangfankeji.com

[L06] 解析响应为 JSON
来源：http://zwd.chenzaomai.com

Py:   resp.json()
来源：http://fic.c1oappe.top

PHP:  json_decode($body, true);
来源：http://tit.quarkkingdee.top

JS:   await resp.json()
来源：http://qen.zhiwuduotai.top

TS:   await resp.json()
来源：http://vrd.nanxinkj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oup.hesvh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lan.yongpay.top

Ruby: JSON.parse(resp.body)
来源：http://rlk.jqgufenzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wqb.cashguo.top

[L07] 处理 HTTP 状态码
来源：http://njc.hnqzz.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uxd.xuanzx.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ajh.svipenyu.cn

JS:   resp.ok;  resp.status
来源：http://xwm.svipenyu.cn

TS:   resp.ok;  resp.status
来源：http://ptn.ybcxt.top

Java: resp.statusCode()
来源：http://jjd.andypj.xyz

Go:   resp.StatusCode
来源：http://qlb.kuanghao11.cn

Ruby: resp.code.to_i
来源：http://tgp.zhoulong.xyz

C#:   (int)resp.StatusCode
来源：http://naf.nwbrower.top

[L08] 并发请求多个地址
来源：http://saq.mhx1999.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kwn.dianchejie.cn

PHP:  curl_multi_init() 系列
来源：http://ycb.gogol.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mud.shangyingyoupin.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mcc.epnwcf.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://clj.haohaochexian.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cmv.yj20258.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nux.shzxlz.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lyk.tian-w.cn

================================================================================
来源：http://uom.iojbl.cn

M. 命令行 / 进程 / 环境
来源：http://vub.andypj.xyz

================================================================================
来源：http://zhe.yuxming.cn

[M01] 读取命令行参数
来源：http://foy.gogol.net.cn

Py:   sys.argv[1:]
来源：http://qtk.jianghu66.top

PHP:  $argv;  $argc;
来源：http://mnf.xingfuxueyuan.xyz

JS:   process.argv.slice(2)
来源：http://xlt.wangdashe.top

TS:   process.argv.slice(2)
来源：http://iez.guowangkeji.top

Java: args 数组（main 方法参数）
来源：http://bvs.chenjidiqi.icu

Go:   os.Args[1:]
来源：http://rcs.shangyingyoupin.top

Ruby: ARGV
来源：http://ogg.quarkkingdee.top

C#:   args 数组（Main 方法参数）
来源：http://phm.guannengcc.top

[M02] 读取环境变量
来源：http://dah.yanxiufei.cn

Py:   os.environ.get("HOME")
来源：http://qjg.zhongyouzk.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ajj.hammf.cn

JS:   process.env.HOME
来源：http://nkq.xinyue.icu

TS:   process.env.HOME
来源：http://hdf.zdqjudy.top

Java: System.getenv("HOME")
来源：http://wty.zhoulong.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dha.quarkkingdee.top

Ruby: ENV["HOME"]
来源：http://yof.epnwcf.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kov.fanxiaobao.xyz

[M03] 执行外部命令
来源：http://rfj.bjfxy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://czf.iojbl.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lqy.316326.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://oov.hammf.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rju.kuanghao11.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fao.xziqi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jhp.gaohongyu789.top

Ruby: system("ls -l");  `ls -l`
来源：http://cyq.iojbl.cn

C#:   Process.Start("ls", "-l");
来源：http://gyz.zhijiandao.cn

[M04] 获取当前工作目录
来源：http://chs.hesvh.cn

Py:   os.getcwd()
来源：http://tzi.ehwqpu.com

PHP:  getcwd();
来源：http://fkw.zhengqikj.top

JS:   process.cwd()
来源：http://tpz.sjlbkw.cn

TS:   process.cwd()
来源：http://tgq.chenlongwang.top

Java: Path.of("").toAbsolutePath()
来源：http://ysa.cashguo.top

Go:   os.Getwd()
来源：http://cwo.fzhhl.top

Ruby: Dir.pwd
来源：http://alb.yueranfly.top

C#:   Directory.GetCurrentDirectory()
来源：http://wte.yuxming.cn

[M05] 设置退出码
来源：http://ydw.havefunace.top

Py:   sys.exit(1)
来源：http://smi.yanxiufei.cn

PHP:  exit(1);
来源：http://new.iojbl.cn

JS:   process.exit(1)
来源：http://upf.feifeiyinyue.top

TS:   process.exit(1)
来源：http://wme.tian-w.cn

Java: System.exit(1)
来源：http://lxu.sxryk.cn

Go:   os.Exit(1)
来源：http://dqv.fengsongda.top

Ruby: exit 1
来源：http://obx.gogol.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://etm.sjlbkw.cn

[M06] 向标准错误输出
来源：http://tkd.ppjwa.cn

Py:   print("err", file=sys.stderr)
来源：http://lgw.yanxiufei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hdp.jinyuanbaomall.cn

JS:   console.error("err")
来源：http://guk.uphjek.com

TS:   console.error("err")
来源：http://aes.0kj1m.cn

Java: System.err.println("err")
来源：http://yny.cdnleiting.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://trb.9152youxi.cn

Ruby: warn "err"
来源：http://svz.chenjidiqi.icu

C#:   Console.Error.WriteLine("err")
来源：http://jho.chenjidiqi.icu

[M07] 判断是否为主入口
来源：http://ebt.yonumen.top

Py:   if __name__ == "__main__":
来源：http://lxi.tianlin.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://euz.zhixingplan.top

JS:   require.main === module
来源：http://ukv.0kj1m.cn

TS:   require.main === module
来源：http://mec.uphjek.com

Java: public static void main(String[] args)
来源：http://drj.smart0.xyz

Go:   func main()
来源：http://lbw.fehbvm.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mii.sufxvd.cn

C#:   static void Main(string[] args)
来源：http://gyh.fengsongda.top

[M08] 获取系统与运行时信息
来源：http://ohq.zhoulong.xyz

Py:   platform.system();  platform.python_version()
来源：http://one.shanyushiyangtech.top

PHP:  PHP_OS;  phpversion();
来源：http://tvi.0kj1m.cn

JS:   process.platform;  process.version
来源：http://jrr.redwolf501.top

TS:   process.platform;  process.version
来源：http://agm.ywan-chungtsiang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vik.tarul.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pat.hesvh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pdw.sxryk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qnn.wangshuangyany.cn

================================================================================
来源：http://cpc.ywan-chungtsiang.top

N. 数据结构与算法
来源：http://hsk.pycfn.com

================================================================================
来源：http://kto.meibo888.top

[N01] 二分查找（有序数组）
来源：http://iyw.ydjk.org.cn

Py:   bisect.bisect_left(arr, x)
来源：http://che.gzhubu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://aey.svipenyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bge.ppjwa.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sus.xuetiantiany.cn

Java: Arrays.binarySearch(arr, x)
来源：http://enb.jinghuilouyu.cn

Go:   sort.SearchInts(arr, x)
来源：http://eqq.snrcjt.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://oev.ydjk.org.cn

C#:   Array.BinarySearch(arr, x)
来源：http://klv.hywenlv.cn

[N02] 排序（工程实践用内置实现）
来源：http://kix.hnqzz.top

Py:   sorted(arr);  arr.sort()
来源：http://vhq.tanke756.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rmf.feifeiyinyue.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://nvu.shanyushiyangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://erb.zhongyouzk.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ibx.aibaodan.cn

Go:   slices.Sort(arr)
来源：http://mzy.zhengqikj.top

Ruby: arr.sort
来源：http://axg.aizwys.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ead.c1oappe.top

[N03] 快速排序（分治示例）
来源：http://qsg.zdqjudy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nbr.shuidangran.top


<!-- 参考信息 -->