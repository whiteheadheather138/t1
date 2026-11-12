代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ieu.dashuyun.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rgc.vehdjk.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uaz.guowangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://eyy.cdnleiting.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rkj.52xcode.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://exi.shuidangran.top

[J05] 时间加减（加 7 天）
来源：http://tbl.xuetiantiany.cn

Py:   now + timedelta(days=7)
来源：http://eok.ywan-chungtsiang.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://sfw.jqgfzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rhe.cdnleiting.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://whb.daxiang520.top

Java: LocalDate.now().plusDays(7)
来源：http://bki.hnxiangtu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ato.zhijiandao.cn

Ruby: Time.now + 7 * 86400
来源：http://ojk.fengsongda.top

C#:   DateTime.Now.AddDays(7)
来源：http://wjq.kuanghao11.cn

[J06] 计算两时间之差
来源：http://dfp.mhx1999.top

Py:   (end - start).total_seconds()
来源：http://hii.yanxiufei.cn

PHP:  $end->diff($start)->days;
来源：http://ofc.feifeiyinyue.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nrm.quarkkingdee.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fyz.xziqi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gkc.zdbjq.cn

Go:   end.Sub(start).Hours()
来源：http://txk.dashuyun.cn

Ruby: end - start                 # 返回秒数
来源：http://scg.yangfankeji.com

C#:   (end - start).TotalSeconds
来源：http://yre.xuetiantiany.cn

[J07] 比较两个日期
来源：http://fgs.sjlbkw.cn

Py:   d1 < d2;  d1 == d2
来源：http://kwr.yangfankeji.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wvd.0kj1m.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nnl.shanyushiyangtech.top

TS:   d1.getTime() < d2.getTime()
来源：http://jgd.zhijiandao.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rbf.fengsongda.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tlp.jqgfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://zsg.gzhubu.top

C#:   d1 < d2;  d1 == d2
来源：http://lds.vehdjk.com

[J08] 提取年月日与星期
来源：http://fgu.zhixingplan.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ugb.vehdjk.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pab.jinghuilouyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vuj.jqgufenzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://aya.daxiang520.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://abd.yj20258.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hno.yvedp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cxg.fengsongda.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fmy.meibo888.top

[J09] 时区处理
来源：http://gra.ydzc1.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ilw.hongshengwenyu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zlm.ydjk.org.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aip.redwolf501.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bir.zhiwuduotai.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rva.xuanzx.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hsz.jiagoushi.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ats.nanxinkj.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lsy.xziqi.cn

[J10] 取今天 / 本月第一天
来源：http://tim.zhongyouzk.top

Py:   date.today();  date.today().replace(day=1)
来源：http://dgs.yj202588.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rdt.dashuyun.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fby.daxiang520.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dlo.xuanzx.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lbc.zhengqikj.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kne.nanxinkj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bvn.feifeiyinyue.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ghy.fzhhl.top

================================================================================
来源：http://uyh.nanxuanxn.top

K. JSON 与序列化
来源：http://yrv.tarul.cn

================================================================================
来源：http://jgy.shangyingyoupin.top

[K01] 对象转 JSON 字符串
来源：http://ypr.zhiwuduotai.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pmx.hesvh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://iyr.jlsjyb.cn

JS:   JSON.stringify(obj)
来源：http://fkp.yanxiufei.cn

TS:   JSON.stringify(obj)
来源：http://gya.chenlongwang.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iuv.yvedp.cn

Go:   json.Marshal(obj)
来源：http://jxn.fengsongda.top

Ruby: obj.to_json                                     // require "json"
来源：http://hta.nanxinkj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://jxk.nanxinkj.top

[K02] JSON 字符串转对象
来源：http://llg.hcnkem.com

Py:   json.loads(s)
来源：http://jqv.yvedp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jga.gaohongyu789.top

JS:   JSON.parse(s)
来源：http://zqp.zhengqikj.top

TS:   JSON.parse(s)
来源：http://cbf.mhx1999.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ocd.yonumen.top

Go:   json.Unmarshal(data, &v)
来源：http://zkc.xziqi.cn

Ruby: JSON.parse(s)
来源：http://ugc.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uja.pengpengdd.cyou

[K03] JSON 美化输出（带缩进）
来源：http://zjn.zhongyouzk.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lpw.cucudq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rma.jinyuanbaomall.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wfv.sysykeji.top

TS:   JSON.stringify(obj, null, 2)
来源：http://osw.sweek.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ayq.shanyushiyangkeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://whe.andypj.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://vco.fzhhl.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bgm.zycfv.cn

[K04] 读取 JSON 文件
来源：http://sxs.ehwqpu.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zdg.zhixingplan.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gbm.hywenlv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wom.0kj1m.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gxp.cashguo.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cqb.birdmap.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rkz.bbcook.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://txl.ydjk.org.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rqm.cheryme.top

[K05] 深拷贝对象
来源：http://uvf.cheryme.top

Py:   copy.deepcopy(obj)
来源：http://kls.jinghuilouyu.cn

PHP:  unserialize(serialize($obj));
来源：http://exk.zycfv.cn

JS:   structuredClone(obj)
来源：http://yuq.meibo888.top

TS:   structuredClone(obj)
来源：http://dcm.yonumen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://nce.sufxvd.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tmd.zhijiandao.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ltk.aizwys.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vhk.yueranfly.top

[K06] 解析 URL 查询串
来源：http://upn.iojbl.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://war.svipenyu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gyc.yanxiufei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://egl.aizwys.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://err.yangfankeji.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cjm.dianchejie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yki.fktsv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://axu.fanxiaobao.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hwo.sweek.top

[K07] 进制转换
来源：http://gpl.shzxlz.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mxx.gaohongyu789.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tbf.jianghu66.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bgl.sxryk.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cjy.tianlin.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qtf.tianlin.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kaj.ybcxt.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://njb.zdqjudy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jfc.mhx1999.top

[K08] 二进制序列化（非 JSON）
来源：http://cke.cdnleiting.top

Py:   pickle.dumps(obj)
来源：http://itu.zhengqikj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://igk.ppjwa.cn

JS:   v8.serialize(obj)        // Node
来源：http://dru.zhijiandao.cn

TS:   v8.serialize(obj)        // Node
来源：http://aub.jianghu66.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xui.zdbjq.cn

Go:   encoding/gob
来源：http://lpt.bbcook.cn

Ruby: Marshal.dump(obj)
来源：http://frt.yanxiufei.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cgc.quarkkingdee.top

================================================================================
来源：http://xqe.hnxiangtu.top

L. 网络请求
来源：http://zkd.hammf.cn

================================================================================
来源：http://ooq.yuxming.cn

[L01] 发送 GET 请求
来源：http://ecz.snrcjt.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vfi.iojbl.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vzf.gogol.net.cn

JS:   await fetch(url)
来源：http://jel.ctjpmb.com

TS:   await fetch(url)
来源：http://ryd.316326.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dps.gzhubu.top

Go:   resp, err := http.Get(url)
来源：http://squ.gzhubu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jyq.epnwcf.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pgy.mhx1999.top

[L02] 发送 POST JSON
来源：http://thm.jianghu66.top

Py:   requests.post(url, json={"a": 1})
来源：http://vfs.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jax.cheryme.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eyj.zhijiandao.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kzc.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://onr.yvedp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dsi.hnqzz.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zxd.jyoumei.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tzk.jiagoushi.top

[L03] 设置自定义请求头
来源：http://nvi.aibaodan.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ltv.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rhc.zhoulong.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fvm.pycfn.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zhm.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://doa.jinyuanbaomall.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dih.316326.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kqr.jianghu66.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tqq.snrcjt.cn

[L04] 设置超时
来源：http://eym.redwolf501.top

Py:   requests.get(url, timeout=5)
来源：http://ebu.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wnp.vehdjk.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kua.zhaomingkeji.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ezo.pycfn.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zxv.yuanzhike.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hly.jinqigufen.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://keg.jinyuanbaomall.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tmf.haohaochexian.top

[L05] 上传文件（multipart）
来源：http://idt.tarul.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://liv.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ckg.havefunace.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pud.zhengqikj.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kts.hnxiangtu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sgo.9152youxi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://azd.hywenlv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jbq.chenzaomai.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yni.sxryk.cn

[L06] 解析响应为 JSON
来源：http://fla.svipenyu.cn

Py:   resp.json()
来源：http://afk.svipenyu.cn

PHP:  json_decode($body, true);
来源：http://ksw.yonumen.top

JS:   await resp.json()
来源：http://har.chenjidiqi.icu

TS:   await resp.json()
来源：http://oez.yj20258888.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bed.haohaochexian.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lnh.nanxuanxn.top

Ruby: JSON.parse(resp.body)
来源：http://mbv.tarul.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mjb.dianchejie.cn

[L07] 处理 HTTP 状态码
来源：http://hhx.zhiwuduotai.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gvg.tianlin.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hrs.zhongyouzk.top

JS:   resp.ok;  resp.status
来源：http://wun.yj202588.top

TS:   resp.ok;  resp.status
来源：http://apf.ivvv.top

Java: resp.statusCode()
来源：http://rps.feifeiyinyue.top

Go:   resp.StatusCode
来源：http://noi.fanxiaobao.xyz

Ruby: resp.code.to_i
来源：http://xqm.hongshengwenyu.top

C#:   (int)resp.StatusCode
来源：http://atj.xinyue.icu

[L08] 并发请求多个地址
来源：http://qnb.zhoulong.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kzi.yvedp.cn

PHP:  curl_multi_init() 系列
来源：http://liv.yj202588.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nqs.yvedp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dfs.gaohongyu789.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mig.gzhubu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yvh.zhengqikj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vti.yuxming.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kda.yanxiufei.cn

================================================================================
来源：http://pmf.guowangkeji.top

M. 命令行 / 进程 / 环境
来源：http://dkh.9152youxi.cn

================================================================================
来源：http://esj.jianghu66.top

[M01] 读取命令行参数
来源：http://ciz.aizwys.cn

Py:   sys.argv[1:]
来源：http://cgl.xuanzx.com

PHP:  $argv;  $argc;
来源：http://mkt.vehdjk.com

JS:   process.argv.slice(2)
来源：http://thz.jinghuilouyu.cn

TS:   process.argv.slice(2)
来源：http://avx.aibaodan.cn

Java: args 数组（main 方法参数）
来源：http://sve.yfazqb.com

Go:   os.Args[1:]
来源：http://upx.zhixingplan.top

Ruby: ARGV
来源：http://qjq.guannengcc.top

C#:   args 数组（Main 方法参数）
来源：http://rfq.aibaodan.cn

[M02] 读取环境变量
来源：http://hpx.ctjpmb.com

Py:   os.environ.get("HOME")
来源：http://tst.hnxiangtu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oxm.hnqzz.top

JS:   process.env.HOME
来源：http://kre.hywenlv.cn

TS:   process.env.HOME
来源：http://tlk.sxryk.cn

Java: System.getenv("HOME")
来源：http://gmj.zhengqikj.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kqv.shuidangran.top

Ruby: ENV["HOME"]
来源：http://upj.hcnkem.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://exv.shanyushiyangkeji.top

[M03] 执行外部命令
来源：http://dib.yanxiufei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yij.jqgufenzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://iiu.gotoacloud.top

JS:   child_process.execSync("ls -l").toString()
来源：http://obb.redwolf501.top

TS:   child_process.execSync("ls -l").toString()
来源：http://red.yfazqb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vur.bjfxy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wdk.ywan-chungtsiang.top

Ruby: system("ls -l");  `ls -l`
来源：http://pfa.vehdjk.com

C#:   Process.Start("ls", "-l");
来源：http://hlt.ctjpmb.com

[M04] 获取当前工作目录
来源：http://khg.sweek.top

Py:   os.getcwd()
来源：http://ctf.vehdjk.com

PHP:  getcwd();
来源：http://xaz.yfazqb.com

JS:   process.cwd()
来源：http://miz.sysykeji.top

TS:   process.cwd()
来源：http://hyc.jinqigufen.top

Java: Path.of("").toAbsolutePath()
来源：http://qci.feifeiyinyue.top

Go:   os.Getwd()
来源：http://trb.daxiang520.top

Ruby: Dir.pwd
来源：http://zcb.vqdsnc.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vjc.yangfankeji.com

[M05] 设置退出码
来源：http://wbe.9152youxi.cn

Py:   sys.exit(1)
来源：http://fxm.zhijiandao.cn

PHP:  exit(1);
来源：http://gko.jyoumei.cn

JS:   process.exit(1)
来源：http://tqn.jyoumei.cn

TS:   process.exit(1)
来源：http://kzr.gaohongyu789.top

Java: System.exit(1)
来源：http://smy.zhiwuduotai.top

Go:   os.Exit(1)
来源：http://kif.ctjpmb.com

Ruby: exit 1
来源：http://gtx.fehbvm.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dqt.nanxinkj.top

[M06] 向标准错误输出
来源：http://sss.shzxlz.cn

Py:   print("err", file=sys.stderr)
来源：http://eyp.ywan-chungtsiang.top

PHP:  fwrite(STDERR, "err\n");
来源：http://etc.yj202588.top

JS:   console.error("err")
来源：http://bnw.ctjpmb.com

TS:   console.error("err")
来源：http://itx.jyoumei.cn

Java: System.err.println("err")
来源：http://nah.daria6918.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bln.nanxuanxn.top

Ruby: warn "err"
来源：http://eah.smart0.xyz

C#:   Console.Error.WriteLine("err")
来源：http://scr.andypj.xyz

[M07] 判断是否为主入口
来源：http://vdu.shanyushiyangkeji.top

Py:   if __name__ == "__main__":
来源：http://kbo.ybcxt.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kmd.yj202588.top

JS:   require.main === module
来源：http://vrx.sufxvd.cn

TS:   require.main === module
来源：http://hgo.chenjidiqi.icu

Java: public static void main(String[] args)
来源：http://irw.aibaodan.cn

Go:   func main()
来源：http://ysu.cheryme.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://osq.meibo888.top

C#:   static void Main(string[] args)
来源：http://tvu.fanxiaobao.xyz

[M08] 获取系统与运行时信息
来源：http://zck.fehbvm.com

Py:   platform.system();  platform.python_version()
来源：http://qub.chenzaomai.com

PHP:  PHP_OS;  phpversion();
来源：http://gjw.meibo888.top

JS:   process.platform;  process.version
来源：http://sfd.jlsjyb.cn

TS:   process.platform;  process.version
来源：http://zlp.smart0.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ccm.tanke756.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tox.jqgufenzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fqs.xuetiantiany.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dbp.feifeiyinyue.top

================================================================================
来源：http://uvx.zycfv.cn

N. 数据结构与算法
来源：http://byf.hysaishi.cn

================================================================================
来源：http://wmq.yj20258888.top

[N01] 二分查找（有序数组）
来源：http://afe.jinqigufen.top

Py:   bisect.bisect_left(arr, x)
来源：http://wxw.sxryk.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kig.redwolf501.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oth.ctjpmb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fwz.nanxinkj.top

Java: Arrays.binarySearch(arr, x)
来源：http://fqi.9152youxi.cn

Go:   sort.SearchInts(arr, x)
来源：http://abr.pengpengdd.cyou

Ruby: arr.bsearch { |e| e >= x }
来源：http://mbb.dianchejie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ahf.smart0.xyz

[N02] 排序（工程实践用内置实现）
来源：http://cue.bbcook.cn

Py:   sorted(arr);  arr.sort()
来源：http://gth.ywan-chungtsiang.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wtk.cucudq.cn


<!-- 参考信息 -->