代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dpc.ehwqpu.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ffj.epnwcf.com

[J05] 时间加减（加 7 天）
来源：http://idw.zhongyouzk.top

Py:   now + timedelta(days=7)
来源：http://vqr.epnwcf.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://bgv.316326.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://evb.mhx1999.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qka.ehwqpu.com

Java: LocalDate.now().plusDays(7)
来源：http://qkt.yanxiufei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bcd.shanyushiyangtech.top

Ruby: Time.now + 7 * 86400
来源：http://ixz.hesvh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dfz.zhengqikj.top

[J06] 计算两时间之差
来源：http://phj.vqdsnc.cn

Py:   (end - start).total_seconds()
来源：http://gik.redwolf501.top

PHP:  $end->diff($start)->days;
来源：http://ita.zhiwuduotai.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ubb.gogol.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://koz.aibaodan.cn

Java: Duration.between(start, end).toSeconds()
来源：http://glj.cheryme.top

Go:   end.Sub(start).Hours()
来源：http://iyh.chenzaomai.com

Ruby: end - start                 # 返回秒数
来源：http://eay.wangdashe.top

C#:   (end - start).TotalSeconds
来源：http://yfs.xuanzx.com

[J07] 比较两个日期
来源：http://qal.hywenlv.cn

Py:   d1 < d2;  d1 == d2
来源：http://ccb.hesvh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hws.xziqi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://iyj.smart0.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://nps.ydjk.org.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xdr.feifeiyinyue.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://thz.yueranfly.top

Ruby: d1 < d2;  d1 == d2
来源：http://hcy.jinyuanbaomall.cn

C#:   d1 < d2;  d1 == d2
来源：http://aiw.zdbjq.cn

[J08] 提取年月日与星期
来源：http://uxj.ehwqpu.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hiz.nanxuanxn.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dkf.iojbl.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hch.guowangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://snv.andypj.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bpa.zhoulong.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dgo.daxiang520.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ltc.zdbjq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jrj.feifeiyinyue.top

[J09] 时区处理
来源：http://fvn.guowangkeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yjr.yj20258888.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wun.yonumen.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jyb.ywan-chungtsiang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://snq.fehbvm.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lgf.hfpthk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xnk.guannengcc.top

Ruby: Time.now.getlocal("+08:00")
来源：http://gzk.daria6918.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://whq.ivvv.top

[J10] 取今天 / 本月第一天
来源：http://sxw.daria6918.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jkp.sweek.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sdn.smart0.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://iza.shzxlz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ocn.xuetiantiany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hsu.tarul.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nyx.jinqigufen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://chk.yuxming.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cvs.xinyue.icu

================================================================================
来源：http://yrp.yj202588.top

K. JSON 与序列化
来源：http://tcv.shangyingyoupin.top

================================================================================
来源：http://xif.tanke756.top

[K01] 对象转 JSON 字符串
来源：http://emf.fanxiaobao.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mfn.svipenyu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xhd.hnqzz.top

JS:   JSON.stringify(obj)
来源：http://dxz.haohaochexian.top

TS:   JSON.stringify(obj)
来源：http://wry.ywan-chungtsiang.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mdq.wangshuangyany.cn

Go:   json.Marshal(obj)
来源：http://vfq.sufxvd.cn

Ruby: obj.to_json                                     // require "json"
来源：http://org.havefunace.top

C#:   JsonSerializer.Serialize(obj)
来源：http://dsx.hongshengwenyu.top

[K02] JSON 字符串转对象
来源：http://bfh.andypj.xyz

Py:   json.loads(s)
来源：http://vgb.hywenlv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ghx.yvedp.cn

JS:   JSON.parse(s)
来源：http://fyi.yanxiufei.cn

TS:   JSON.parse(s)
来源：http://mxo.dianchejie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ebg.yvedp.cn

Go:   json.Unmarshal(data, &v)
来源：http://kdq.316326.xyz

Ruby: JSON.parse(s)
来源：http://iye.shangyingyoupin.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qxp.smart0.xyz

[K03] JSON 美化输出（带缩进）
来源：http://pip.zhixingplan.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kvj.kuanghao11.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://igk.yongpay.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hnn.zhiwuduotai.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hob.xuanzx.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://anu.gotoacloud.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vdc.ehwqpu.com

Ruby: JSON.pretty_generate(obj)
来源：http://tbh.sxryk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fbe.zhixingplan.top

[K04] 读取 JSON 文件
来源：http://ocg.fktsv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://swt.cashguo.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wuv.zhaomingkeji.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gnq.guannengcc.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fkj.chenlongwang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vbf.gaohongyu789.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cob.hesvh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://iyb.wangdashe.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://poj.zhongyouzk.top

[K05] 深拷贝对象
来源：http://jxc.jinqigufen.top

Py:   copy.deepcopy(obj)
来源：http://bzg.yj20258.top

PHP:  unserialize(serialize($obj));
来源：http://xus.feifeiyinyue.top

JS:   structuredClone(obj)
来源：http://gxn.hnxiangtu.top

TS:   structuredClone(obj)
来源：http://odg.bjfxy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://euf.gaohongyu789.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rtu.9152youxi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yzq.cucudq.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cae.52xcode.cn

[K06] 解析 URL 查询串
来源：http://car.bbcook.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tcz.aizwys.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://paj.ivvv.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dod.gotoacloud.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nji.snrcjt.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lep.yuanzhike.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://tus.birdmap.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vjx.svipenyu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fue.yangfankeji.com

[K07] 进制转换
来源：http://iqv.shanyushiyangtech.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wbr.zhoulong.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rxh.c1oappe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xhu.chenlongwang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zoc.yj20258888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wia.xuanzx.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bvm.yj20258888.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pka.0kj1m.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fdk.shanyushiyangtech.top

[K08] 二进制序列化（非 JSON）
来源：http://opz.smart0.xyz

Py:   pickle.dumps(obj)
来源：http://lmf.tian-w.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://net.fzhhl.top

JS:   v8.serialize(obj)        // Node
来源：http://kka.jinqigufen.top

TS:   v8.serialize(obj)        // Node
来源：http://doz.aizwys.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uxn.zhongyouzk.top

Go:   encoding/gob
来源：http://ikg.pycfn.com

Ruby: Marshal.dump(obj)
来源：http://fml.feifeiyinyue.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vmn.daria6918.cn

================================================================================
来源：http://rgd.316326.xyz

L. 网络请求
来源：http://cbi.chenzaomai.com

================================================================================
来源：http://owq.jqgfzy.top

[L01] 发送 GET 请求
来源：http://kla.jinyuanbaomall.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ewk.dashuyun.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qde.hywenlv.cn

JS:   await fetch(url)
来源：http://qpw.zhongyouzk.top

TS:   await fetch(url)
来源：http://fao.cqqwz.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mwx.bbcook.cn

Go:   resp, err := http.Get(url)
来源：http://pzj.jinqigufen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://fkt.shanyushiyangkeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dak.haohaochexian.top

[L02] 发送 POST JSON
来源：http://toq.c1oappe.top

Py:   requests.post(url, json={"a": 1})
来源：http://lie.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://egl.zhijiandao.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nsb.zhongyouzk.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qeq.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yyn.hysaishi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kwz.andypj.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qus.yj20258.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oae.bjfxy.top

[L03] 设置自定义请求头
来源：http://mal.pengpengdd.cyou

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vpk.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cgz.bbcook.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://prb.zhaomingkeji.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://izf.yanxiufei.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ofl.mhx1999.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ypk.yueranfly.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yog.sysykeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pvk.hcnkem.com

[L04] 设置超时
来源：http://uba.shuidangran.top

Py:   requests.get(url, timeout=5)
来源：http://sjp.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tbt.pengpengdd.cyou

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dtc.wangshuangyany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nop.cheryme.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://psi.cdnleiting.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fbw.meibo888.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dxb.sxryk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gjw.birdmap.top

[L05] 上传文件（multipart）
来源：http://rbb.gaohongyu789.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rkg.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dyc.yvedp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zxz.yanxiufei.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://flv.shuidangran.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dst.hcnkem.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kgf.birdmap.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ito.wangdashe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zxx.chenzaomai.com

[L06] 解析响应为 JSON
来源：http://xlb.ivvv.top

Py:   resp.json()
来源：http://xlp.pengpengdd.cyou

PHP:  json_decode($body, true);
来源：http://uim.vehdjk.com

JS:   await resp.json()
来源：http://gys.0kj1m.cn

TS:   await resp.json()
来源：http://red.jinqigufen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kqv.daria6918.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qov.xziqi.cn

Ruby: JSON.parse(resp.body)
来源：http://jbw.xinyue.icu

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jxt.hesvh.cn

[L07] 处理 HTTP 状态码
来源：http://vkw.316326.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bfg.ybcxt.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ccq.hfpthk.cn

JS:   resp.ok;  resp.status
来源：http://vdx.cheryme.top

TS:   resp.ok;  resp.status
来源：http://odh.9152youxi.cn

Java: resp.statusCode()
来源：http://hjp.tanke756.top

Go:   resp.StatusCode
来源：http://uzy.aibaodan.cn

Ruby: resp.code.to_i
来源：http://qlp.zhaomingkeji.xyz

C#:   (int)resp.StatusCode
来源：http://xcg.xuetiantiany.cn

[L08] 并发请求多个地址
来源：http://fhi.jlsjyb.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kyf.cqqwz.cn

PHP:  curl_multi_init() 系列
来源：http://mce.316326.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ybb.guowangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yac.hnxiangtu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://egv.yj202588.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fug.bbcook.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lgn.dashuyun.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xbb.bbcook.cn

================================================================================
来源：http://jzb.fengsongda.top

M. 命令行 / 进程 / 环境
来源：http://avj.aizwys.cn

================================================================================
来源：http://rxk.hcnkem.com

[M01] 读取命令行参数
来源：http://dsd.jinyuanbaomall.cn

Py:   sys.argv[1:]
来源：http://vyw.zhongyouzk.top

PHP:  $argv;  $argc;
来源：http://fio.316326.xyz

JS:   process.argv.slice(2)
来源：http://sni.nwbrower.top

TS:   process.argv.slice(2)
来源：http://yru.zhiwuduotai.top

Java: args 数组（main 方法参数）
来源：http://vpf.yongpay.top

Go:   os.Args[1:]
来源：http://sdd.jinqigufen.top

Ruby: ARGV
来源：http://ljz.316326.xyz

C#:   args 数组（Main 方法参数）
来源：http://cse.fengsongda.top

[M02] 读取环境变量
来源：http://osa.pengpengdd.cyou

Py:   os.environ.get("HOME")
来源：http://myb.ybcxt.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xak.snrcjt.cn

JS:   process.env.HOME
来源：http://pst.gogol.net.cn

TS:   process.env.HOME
来源：http://iss.guannengcc.top

Java: System.getenv("HOME")
来源：http://wos.daria6918.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sod.yuxming.cn

Ruby: ENV["HOME"]
来源：http://gby.yuanzhike.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ndg.aizwys.cn

[M03] 执行外部命令
来源：http://zsl.xziqi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cio.shanyushiyangkeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zgc.kuanghao11.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yfo.tianlin.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://jqq.nwbrower.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yhd.jqgfzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://yxv.ywan-chungtsiang.top

Ruby: system("ls -l");  `ls -l`
来源：http://btl.shanyushiyangtech.top

C#:   Process.Start("ls", "-l");
来源：http://gkl.xziqi.cn

[M04] 获取当前工作目录
来源：http://zfd.dashuyun.cn

Py:   os.getcwd()
来源：http://wcp.hcnkem.com

PHP:  getcwd();
来源：http://gki.gotoacloud.top

JS:   process.cwd()
来源：http://ltm.pycfn.com

TS:   process.cwd()
来源：http://qib.yfazqb.com

Java: Path.of("").toAbsolutePath()
来源：http://ezw.tian-w.cn

Go:   os.Getwd()
来源：http://xdb.xuetiantiany.cn

Ruby: Dir.pwd
来源：http://hlm.aibaodan.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xwp.uphjek.com

[M05] 设置退出码
来源：http://ukb.hammf.cn

Py:   sys.exit(1)
来源：http://xuu.tarul.cn

PHP:  exit(1);
来源：http://xci.havefunace.top

JS:   process.exit(1)
来源：http://bkb.ybcxt.top

TS:   process.exit(1)
来源：http://ief.birdmap.top

Java: System.exit(1)
来源：http://oro.yfazqb.com

Go:   os.Exit(1)
来源：http://oif.ybcxt.top

Ruby: exit 1
来源：http://eth.guowangkeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://epv.nanxinkj.top

[M06] 向标准错误输出
来源：http://wkh.xinyue.icu

Py:   print("err", file=sys.stderr)
来源：http://wka.jinghuilouyu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lrk.shanyushiyangkeji.top

JS:   console.error("err")
来源：http://oql.yonumen.top

TS:   console.error("err")
来源：http://zqo.shangyingyoupin.top

Java: System.err.println("err")
来源：http://wrr.cqqwz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://eah.zhiwuduotai.top

Ruby: warn "err"
来源：http://ngk.xuanzx.com

C#:   Console.Error.WriteLine("err")
来源：http://xmw.gaohongyu789.top

[M07] 判断是否为主入口
来源：http://nil.fzhhl.top

Py:   if __name__ == "__main__":
来源：http://nxn.xziqi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bwi.chenjidiqi.icu

JS:   require.main === module
来源：http://ghh.shanyushiyangtech.top

TS:   require.main === module
来源：http://skx.jinghuilouyu.cn

Java: public static void main(String[] args)
来源：http://apt.xuanzx.com

Go:   func main()
来源：http://shf.kuanghao11.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tsi.wangdashe.top

C#:   static void Main(string[] args)
来源：http://rfo.aizwys.cn

[M08] 获取系统与运行时信息
来源：http://elj.shanyushiyangtech.top

Py:   platform.system();  platform.python_version()
来源：http://udh.yonumen.top

PHP:  PHP_OS;  phpversion();
来源：http://nzb.sysykeji.top

JS:   process.platform;  process.version
来源：http://kua.kuanghao11.cn

TS:   process.platform;  process.version
来源：http://dhq.smart0.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hbh.sufxvd.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wba.c1oappe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zax.snrcjt.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cwc.ybcxt.top

================================================================================
来源：http://oqr.fzhhl.top

N. 数据结构与算法
来源：http://zry.sxryk.cn

================================================================================
来源：http://xyt.meibo888.top

[N01] 二分查找（有序数组）
来源：http://ref.ywan-chungtsiang.top

Py:   bisect.bisect_left(arr, x)
来源：http://hov.wangdashe.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ene.daria6918.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://roh.yonumen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bdj.cdnleiting.top

Java: Arrays.binarySearch(arr, x)
来源：http://uka.jinqigufen.top

Go:   sort.SearchInts(arr, x)
来源：http://yoi.hnxiangtu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://whr.gzhubu.top

C#:   Array.BinarySearch(arr, x)
来源：http://cda.guowangkeji.top

[N02] 排序（工程实践用内置实现）
来源：http://qlx.aibaodan.cn

Py:   sorted(arr);  arr.sort()
来源：http://crd.zhaomingkeji.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fvj.xylfe.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://foj.gogol.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sqr.shanyushiyangtech.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tjj.cheryme.top

Go:   slices.Sort(arr)
来源：http://req.yangfankeji.com


<!-- 参考信息 -->