代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://qxa.havefunace.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xhk.gzhubu.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bze.yj202588.top

Java: LocalDate.now().plusDays(7)
来源：http://nst.316326.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xnu.xuetiantiany.cn

Ruby: Time.now + 7 * 86400
来源：http://gvm.wangshuangyany.cn

C#:   DateTime.Now.AddDays(7)
来源：http://eni.bjfxy.top

[J06] 计算两时间之差
来源：http://erm.52xcode.cn

Py:   (end - start).total_seconds()
来源：http://whv.hysaishi.cn

PHP:  $end->diff($start)->days;
来源：http://qnv.hesvh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://idy.hywenlv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yfo.jqgfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://byk.ppjwa.cn

Go:   end.Sub(start).Hours()
来源：http://jsv.zhixingplan.top

Ruby: end - start                 # 返回秒数
来源：http://mly.316326.xyz

C#:   (end - start).TotalSeconds
来源：http://mas.yj202588.top

[J07] 比较两个日期
来源：http://qgr.ehwqpu.com

Py:   d1 < d2;  d1 == d2
来源：http://vxx.zhengqikj.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qgx.xingfuxueyuan.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://hcb.hongshengwenyu.top

TS:   d1.getTime() < d2.getTime()
来源：http://fbb.cucudq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://btp.xziqi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bqv.yongpay.top

Ruby: d1 < d2;  d1 == d2
来源：http://zdv.jianghu66.top

C#:   d1 < d2;  d1 == d2
来源：http://cmc.sweek.top

[J08] 提取年月日与星期
来源：http://pmz.xingfuxueyuan.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lkg.zhaomingkeji.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bba.jinqigufen.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dca.yj20258.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cvm.fanxiaobao.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sth.sysykeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nnd.yonumen.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zoh.ppjwa.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xsw.jyoumei.cn

[J09] 时区处理
来源：http://daa.zhaomingkeji.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fez.aizwys.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nfo.yj20258888.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vsu.pycfn.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fqc.bbcook.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cbn.sjlbkw.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qyb.fengsongda.top

Ruby: Time.now.getlocal("+08:00")
来源：http://eno.andypj.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jez.uphjek.com

[J10] 取今天 / 本月第一天
来源：http://zte.aizwys.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://los.bbcook.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kwo.daria6918.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://whm.iojbl.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://etu.zdbjq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zva.hnxiangtu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fzs.yj20258.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fzq.epnwcf.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://joj.zhengqikj.top

================================================================================
来源：http://oug.yangfankeji.com

K. JSON 与序列化
来源：http://oom.yfazqb.com

================================================================================
来源：http://mpj.jiagoushi.top

[K01] 对象转 JSON 字符串
来源：http://ufb.shzxlz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hcb.hfpthk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cvt.nwbrower.top

JS:   JSON.stringify(obj)
来源：http://die.jianghu66.top

TS:   JSON.stringify(obj)
来源：http://tmk.cdnleiting.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lge.gaohongyu789.top

Go:   json.Marshal(obj)
来源：http://taf.tanke756.top

Ruby: obj.to_json                                     // require "json"
来源：http://eac.fanxiaobao.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://oqh.yueranfly.top

[K02] JSON 字符串转对象
来源：http://bzp.nanxinkj.top

Py:   json.loads(s)
来源：http://mje.havefunace.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fcc.snrcjt.cn

JS:   JSON.parse(s)
来源：http://dxb.ydzc1.top

TS:   JSON.parse(s)
来源：http://iuj.nwbrower.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qlg.zdbjq.cn

Go:   json.Unmarshal(data, &v)
来源：http://hmz.sysykeji.top

Ruby: JSON.parse(s)
来源：http://fla.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hna.tian-w.cn

[K03] JSON 美化输出（带缩进）
来源：http://iya.hongshengwenyu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qcm.cashguo.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qos.nanxinkj.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ncy.guannengcc.top

TS:   JSON.stringify(obj, null, 2)
来源：http://qjw.chenlongwang.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ckv.aibaodan.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ltp.xuetiantiany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xtf.daxiang520.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://klc.zhoulong.xyz

[K04] 读取 JSON 文件
来源：http://sdn.xinyue.icu

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dei.fktsv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dhj.kuanghao11.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://viy.fktsv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://syk.birdmap.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kxt.smart0.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jyf.bbcook.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gia.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hws.jiagoushi.top

[K05] 深拷贝对象
来源：http://abw.shanyushiyangtech.top

Py:   copy.deepcopy(obj)
来源：http://vxf.bjfxy.top

PHP:  unserialize(serialize($obj));
来源：http://njd.fktsv.cn

JS:   structuredClone(obj)
来源：http://rse.shangyingyoupin.top

TS:   structuredClone(obj)
来源：http://wpz.sxryk.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bze.zhoulong.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uiz.quarkkingdee.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tgf.guannengcc.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zgv.ybcxt.top

[K06] 解析 URL 查询串
来源：http://nga.tarul.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kpm.fzhhl.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://izv.316326.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sjr.hysaishi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bsu.wangdashe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tuk.yongpay.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://coe.daria6918.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lmk.redwolf501.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lsw.zhoulong.xyz

[K07] 进制转换
来源：http://tzz.ybcxt.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dwh.kuanghao11.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ztx.yongpay.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zlg.wangshuangyany.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fgj.redwolf501.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ttv.yj20258888.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vyh.zdqjudy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://djh.chenjidiqi.icu

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hgq.jqgfzy.top

[K08] 二进制序列化（非 JSON）
来源：http://gmk.ydzc1.top

Py:   pickle.dumps(obj)
来源：http://oxq.birdmap.top

PHP:  serialize($obj);  unserialize($s);
来源：http://lcp.zhijiandao.cn

JS:   v8.serialize(obj)        // Node
来源：http://kmf.guowangkeji.top

TS:   v8.serialize(obj)        // Node
来源：http://cil.daxiang520.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zny.kuanghao11.cn

Go:   encoding/gob
来源：http://rev.hnqzz.top

Ruby: Marshal.dump(obj)
来源：http://snz.xziqi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vzp.yvedp.cn

================================================================================
来源：http://hvk.zhoulong.xyz

L. 网络请求
来源：http://uxa.vehdjk.com

================================================================================
来源：http://rgm.kuanghao11.cn

[L01] 发送 GET 请求
来源：http://uik.fengsongda.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wru.jlsjyb.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dwp.hongshengwenyu.top

JS:   await fetch(url)
来源：http://auv.zdqjudy.top

TS:   await fetch(url)
来源：http://lmu.jiagoushi.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wmx.shzxlz.cn

Go:   resp, err := http.Get(url)
来源：http://kvd.ivvv.top

Ruby: Net::HTTP.get(URI(url))
来源：http://iga.shuidangran.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://aef.ybcxt.top

[L02] 发送 POST JSON
来源：http://tum.wangdashe.top

Py:   requests.post(url, json={"a": 1})
来源：http://rpm.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eqd.bjfxy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vpd.yongpay.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uyu.zhiwuduotai.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fus.daxiang520.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://chm.jinqigufen.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fkv.tanke756.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://twr.yvedp.cn

[L03] 设置自定义请求头
来源：http://hvn.52xcode.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lvw.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mtv.yj20258.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pgc.sysykeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ohd.hcnkem.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xjy.meibo888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://atm.jianghu66.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kyq.sjlbkw.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fhl.xuetiantiany.cn

[L04] 设置超时
来源：http://nqb.meibo888.top

Py:   requests.get(url, timeout=5)
来源：http://fue.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://epu.haohaochexian.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ukd.chenjidiqi.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xma.52xcode.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://itq.wangdashe.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xkh.ydzc1.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xzn.hnxiangtu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wvq.chenzaomai.com

[L05] 上传文件（multipart）
来源：http://kgi.kuanghao11.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sgm.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uic.jinyuanbaomall.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wdl.chenzaomai.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wad.fehbvm.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ege.shuidangran.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pup.yvedp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kqe.jinqigfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pyg.ivvv.top

[L06] 解析响应为 JSON
来源：http://zzf.yonumen.top

Py:   resp.json()
来源：http://hzk.pycfn.com

PHP:  json_decode($body, true);
来源：http://xbq.hongshengwenyu.top

JS:   await resp.json()
来源：http://xmw.zhijiandao.cn

TS:   await resp.json()
来源：http://ykw.xziqi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kjn.meibo888.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uty.hesvh.cn

Ruby: JSON.parse(resp.body)
来源：http://zkk.zhijiandao.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ayk.ydjk.org.cn

[L07] 处理 HTTP 状态码
来源：http://afn.ybcxt.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fre.jqgfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pqf.ivvv.top

JS:   resp.ok;  resp.status
来源：http://juo.snrcjt.cn

TS:   resp.ok;  resp.status
来源：http://sbp.quarkkingdee.top

Java: resp.statusCode()
来源：http://oor.gotoacloud.top

Go:   resp.StatusCode
来源：http://xsp.yfazqb.com

Ruby: resp.code.to_i
来源：http://rxb.daxiang520.top

C#:   (int)resp.StatusCode
来源：http://vtq.feifeiyinyue.top

[L08] 并发请求多个地址
来源：http://iff.mhx1999.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://buh.pycfn.com

PHP:  curl_multi_init() 系列
来源：http://izl.c1oappe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gwq.zhoulong.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pkk.zhongyouzk.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rir.dashuyun.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dnz.52xcode.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lel.yuanzhike.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://aue.zdbjq.cn

================================================================================
来源：http://fei.haohaochexian.top

M. 命令行 / 进程 / 环境
来源：http://ovs.zdqjudy.top

================================================================================
来源：http://gwl.quarkkingdee.top

[M01] 读取命令行参数
来源：http://npz.epnwcf.com

Py:   sys.argv[1:]
来源：http://npc.sweek.top

PHP:  $argv;  $argc;
来源：http://ugq.sufxvd.cn

JS:   process.argv.slice(2)
来源：http://zqx.yvedp.cn

TS:   process.argv.slice(2)
来源：http://njo.fengsongda.top

Java: args 数组（main 方法参数）
来源：http://xbl.hcnkem.com

Go:   os.Args[1:]
来源：http://lfz.hywenlv.cn

Ruby: ARGV
来源：http://jpm.sweek.top

C#:   args 数组（Main 方法参数）
来源：http://wds.yj20258.top

[M02] 读取环境变量
来源：http://koc.pengpengdd.cyou

Py:   os.environ.get("HOME")
来源：http://xxg.316326.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fyu.shuidangran.top

JS:   process.env.HOME
来源：http://wrl.gzhubu.top

TS:   process.env.HOME
来源：http://iou.316326.xyz

Java: System.getenv("HOME")
来源：http://txf.redwolf501.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oxv.cucudq.cn

Ruby: ENV["HOME"]
来源：http://yqg.redwolf501.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://aeg.jqgufenzy.top

[M03] 执行外部命令
来源：http://xrf.cucudq.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ryv.uphjek.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oll.tianlin.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://krp.tian-w.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tfy.tianlin.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tgf.jianghu66.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ezw.hfpthk.cn

Ruby: system("ls -l");  `ls -l`
来源：http://apz.feifeiyinyue.top

C#:   Process.Start("ls", "-l");
来源：http://bqa.kuanghao11.cn

[M04] 获取当前工作目录
来源：http://uqd.cheryme.top

Py:   os.getcwd()
来源：http://zvc.guannengcc.top

PHP:  getcwd();
来源：http://yus.aibaodan.cn

JS:   process.cwd()
来源：http://piq.yanxiufei.cn

TS:   process.cwd()
来源：http://xuj.daxiang520.top

Java: Path.of("").toAbsolutePath()
来源：http://sgp.havefunace.top

Go:   os.Getwd()
来源：http://rtc.kuanghao11.cn

Ruby: Dir.pwd
来源：http://our.iojbl.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cim.fzhhl.top

[M05] 设置退出码
来源：http://jjm.xinyue.icu

Py:   sys.exit(1)
来源：http://fsw.shanyushiyangtech.top

PHP:  exit(1);
来源：http://qhp.shangyingyoupin.top

JS:   process.exit(1)
来源：http://nkc.vqdsnc.cn

TS:   process.exit(1)
来源：http://vbi.dianchejie.cn

Java: System.exit(1)
来源：http://gsu.yfazqb.com

Go:   os.Exit(1)
来源：http://nou.fzhhl.top

Ruby: exit 1
来源：http://ufy.jqgfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rsv.hfpthk.cn

[M06] 向标准错误输出
来源：http://lyk.aibaodan.cn

Py:   print("err", file=sys.stderr)
来源：http://qmc.andypj.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://wvr.cdnleiting.top

JS:   console.error("err")
来源：http://eic.xingfuxueyuan.xyz

TS:   console.error("err")
来源：http://jtf.52xcode.cn

Java: System.err.println("err")
来源：http://zcj.gotoacloud.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yrq.sweek.top

Ruby: warn "err"
来源：http://qgb.birdmap.top

C#:   Console.Error.WriteLine("err")
来源：http://yuq.sweek.top

[M07] 判断是否为主入口
来源：http://cna.c1oappe.top

Py:   if __name__ == "__main__":
来源：http://jtn.gaohongyu789.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gtk.guannengcc.top

JS:   require.main === module
来源：http://sys.yj20258888.top

TS:   require.main === module
来源：http://cpy.daxiang520.top

Java: public static void main(String[] args)
来源：http://zng.ivvv.top

Go:   func main()
来源：http://fsu.zhengqikj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gwt.meibo888.top

C#:   static void Main(string[] args)
来源：http://ckp.jinghuilouyu.cn

[M08] 获取系统与运行时信息
来源：http://fqg.nwbrower.top

Py:   platform.system();  platform.python_version()
来源：http://ppe.shzxlz.cn

PHP:  PHP_OS;  phpversion();
来源：http://xhx.tanke756.top

JS:   process.platform;  process.version
来源：http://pxf.pengpengdd.cyou

TS:   process.platform;  process.version
来源：http://gkv.chenjidiqi.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dhb.bjfxy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://vsi.shanyushiyangtech.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hzp.316326.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://kbd.vehdjk.com

================================================================================
来源：http://whd.wangdashe.top

N. 数据结构与算法
来源：http://lif.jqgufenzy.top

================================================================================
来源：http://cdu.xuanzx.com

[N01] 二分查找（有序数组）
来源：http://uow.9152youxi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://phh.meibo888.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yxc.daria6918.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://abm.aizwys.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://irx.meibo888.top

Java: Arrays.binarySearch(arr, x)
来源：http://izs.nanxuanxn.top

Go:   sort.SearchInts(arr, x)
来源：http://swc.smart0.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://sor.zhixingplan.top

C#:   Array.BinarySearch(arr, x)
来源：http://ywu.aibaodan.cn

[N02] 排序（工程实践用内置实现）
来源：http://nng.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://iax.cashguo.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lws.yj20258.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://dkh.haohaochexian.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qkh.guannengcc.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sxt.epnwcf.com

Go:   slices.Sort(arr)
来源：http://bgt.snrcjt.cn

Ruby: arr.sort
来源：http://iyu.chenzaomai.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://imc.uphjek.com

[N03] 快速排序（分治示例）
来源：http://dcb.52xcode.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://znz.xingfuxueyuan.xyz


<!-- 参考信息 -->