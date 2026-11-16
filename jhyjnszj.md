代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qqb.jqgufenzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ojz.yuanzhike.top

[J05] 时间加减（加 7 天）
来源：http://sdj.fehbvm.com

Py:   now + timedelta(days=7)
来源：http://bwu.pengpengdd.cyou

PHP:  (new DateTime())->modify("+7 days");
来源：http://tus.yuxming.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bmz.zycfv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vhz.pengpengdd.cyou

Java: LocalDate.now().plusDays(7)
来源：http://omu.ydzc1.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gtq.yueranfly.top

Ruby: Time.now + 7 * 86400
来源：http://jtt.ehwqpu.com

C#:   DateTime.Now.AddDays(7)
来源：http://fpa.9152youxi.cn

[J06] 计算两时间之差
来源：http://hqb.jqgfzy.top

Py:   (end - start).total_seconds()
来源：http://huc.nanxuanxn.top

PHP:  $end->diff($start)->days;
来源：http://twh.jianghu66.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ots.daxiang520.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://plb.ppjwa.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bdh.yangfankeji.com

Go:   end.Sub(start).Hours()
来源：http://yju.svipenyu.cn

Ruby: end - start                 # 返回秒数
来源：http://cqp.yj20258888.top

C#:   (end - start).TotalSeconds
来源：http://ftw.fengsongda.top

[J07] 比较两个日期
来源：http://iki.sysykeji.top

Py:   d1 < d2;  d1 == d2
来源：http://cvg.hysaishi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dct.zhoulong.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://jjs.fehbvm.com

TS:   d1.getTime() < d2.getTime()
来源：http://clc.cheryme.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ndp.kuanghao11.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ufi.yongpay.top

Ruby: d1 < d2;  d1 == d2
来源：http://odq.gaohongyu789.top

C#:   d1 < d2;  d1 == d2
来源：http://yyu.0kj1m.cn

[J08] 提取年月日与星期
来源：http://uwr.cheryme.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jwr.zdqjudy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cwn.yj202588.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iru.jqgufenzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kxx.ivvv.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vro.iojbl.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uvp.bbcook.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uem.aizwys.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ody.daria6918.cn

[J09] 时区处理
来源：http://ymo.vehdjk.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://akv.hfpthk.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wwt.hnqzz.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eoh.shuidangran.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xxy.gaohongyu789.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ugh.zdbjq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vwz.haohaochexian.top

Ruby: Time.now.getlocal("+08:00")
来源：http://sns.jinqigufen.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jiu.tian-w.cn

[J10] 取今天 / 本月第一天
来源：http://gps.ppjwa.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ywd.shangyingyoupin.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xyr.mhx1999.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lsc.aizwys.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tgy.ivvv.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jeq.jiagoushi.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cpy.tarul.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://thd.epnwcf.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eys.nanxinkj.top

================================================================================
来源：http://bke.nanxinkj.top

K. JSON 与序列化
来源：http://yei.yvedp.cn

================================================================================
来源：http://mal.xziqi.cn

[K01] 对象转 JSON 字符串
来源：http://ydj.gaohongyu789.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ofs.svipenyu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dpo.yj20258888.top

JS:   JSON.stringify(obj)
来源：http://fas.cqqwz.cn

TS:   JSON.stringify(obj)
来源：http://sgb.cheryme.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qzw.havefunace.top

Go:   json.Marshal(obj)
来源：http://pxc.yonumen.top

Ruby: obj.to_json                                     // require "json"
来源：http://xrd.shuidangran.top

C#:   JsonSerializer.Serialize(obj)
来源：http://iyy.daxiang520.top

[K02] JSON 字符串转对象
来源：http://ycy.zhengqikj.top

Py:   json.loads(s)
来源：http://ofn.yueranfly.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://omz.ybcxt.top

JS:   JSON.parse(s)
来源：http://itw.wangdashe.top

TS:   JSON.parse(s)
来源：http://onk.jiagoushi.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qar.sweek.top

Go:   json.Unmarshal(data, &v)
来源：http://nph.zdbjq.cn

Ruby: JSON.parse(s)
来源：http://ffv.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tit.jianghu66.top

[K03] JSON 美化输出（带缩进）
来源：http://gmd.jqgufenzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fhm.daxiang520.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xbu.zycfv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://seb.pengpengdd.cyou

TS:   JSON.stringify(obj, null, 2)
来源：http://xrx.iojbl.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dkf.ctjpmb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kmy.xuetiantiany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gfz.zhongyouzk.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://czs.9152youxi.cn

[K04] 读取 JSON 文件
来源：http://yeu.xuetiantiany.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://keb.snrcjt.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uji.fktsv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gmv.zhaomingkeji.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cne.fktsv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ydf.hnqzz.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cbv.yj20258.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://dtu.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nsx.fzhhl.top

[K05] 深拷贝对象
来源：http://iwx.wangshuangyany.cn

Py:   copy.deepcopy(obj)
来源：http://fam.gaohongyu789.top

PHP:  unserialize(serialize($obj));
来源：http://bjw.yonumen.top

JS:   structuredClone(obj)
来源：http://wua.jqgfzy.top

TS:   structuredClone(obj)
来源：http://mlh.bbcook.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gof.zycfv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cfa.nanxinkj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tlo.gogol.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xnk.mhx1999.top

[K06] 解析 URL 查询串
来源：http://tcy.xinyue.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cds.jiagoushi.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ogu.jinyuanbaomall.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fmz.hcnkem.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ash.vqdsnc.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wgs.dianchejie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fjo.yfazqb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://srt.cucudq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zyo.yuxming.cn

[K07] 进制转换
来源：http://jfe.ybcxt.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bzu.yj202588.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jys.hesvh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gkg.zycfv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ggl.iojbl.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://big.havefunace.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fks.pycfn.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://acu.sysykeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tkk.zycfv.cn

[K08] 二进制序列化（非 JSON）
来源：http://eth.zhixingplan.top

Py:   pickle.dumps(obj)
来源：http://uux.gzhubu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://gpn.tanke756.top

JS:   v8.serialize(obj)        // Node
来源：http://zfs.quarkkingdee.top

TS:   v8.serialize(obj)        // Node
来源：http://eap.yfazqb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dby.svipenyu.cn

Go:   encoding/gob
来源：http://eem.ehwqpu.com

Ruby: Marshal.dump(obj)
来源：http://kuo.zhengqikj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mnp.jinghuilouyu.cn

================================================================================
来源：http://jhv.xuetiantiany.cn

L. 网络请求
来源：http://tbp.ydjk.org.cn

================================================================================
来源：http://gtb.gotoacloud.top

[L01] 发送 GET 请求
来源：http://aaa.zhixingplan.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fxa.yongpay.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fxx.jinqigfzy.top

JS:   await fetch(url)
来源：http://oql.shanyushiyangtech.top

TS:   await fetch(url)
来源：http://mun.gzhubu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ruq.yonumen.top

Go:   resp, err := http.Get(url)
来源：http://erz.cheryme.top

Ruby: Net::HTTP.get(URI(url))
来源：http://xym.daxiang520.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pex.yj20258888.top

[L02] 发送 POST JSON
来源：http://clk.bjfxy.top

Py:   requests.post(url, json={"a": 1})
来源：http://cah.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://heb.cashguo.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://liy.zycfv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vfw.cdnleiting.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dqg.meibo888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sbg.jinqigufen.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qft.yuanzhike.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lmt.epnwcf.com

[L03] 设置自定义请求头
来源：http://btm.hcnkem.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hdz.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tvp.yfazqb.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yos.meibo888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dzv.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tcx.jinqigufen.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ued.cdnleiting.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zsw.cashguo.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qtn.shuidangran.top

[L04] 设置超时
来源：http://ciw.cdnleiting.top

Py:   requests.get(url, timeout=5)
来源：http://ftn.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dsb.xuanzx.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kdi.yvedp.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eem.dianchejie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://imt.kuanghao11.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cat.daxiang520.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://erc.cashguo.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jou.guannengcc.top

[L05] 上传文件（multipart）
来源：http://ubv.zhixingplan.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zwy.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jyh.tian-w.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pnm.kuanghao11.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rll.tanke756.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fvn.hcnkem.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qyq.xinyue.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jrd.hammf.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cmz.daria6918.cn

[L06] 解析响应为 JSON
来源：http://qme.zycfv.cn

Py:   resp.json()
来源：http://clz.jyoumei.cn

PHP:  json_decode($body, true);
来源：http://eik.shzxlz.cn

JS:   await resp.json()
来源：http://xww.jinqigufen.top

TS:   await resp.json()
来源：http://sgo.yuxming.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://don.sjlbkw.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ugb.hesvh.cn

Ruby: JSON.parse(resp.body)
来源：http://lal.dashuyun.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sgc.jqgfzy.top

[L07] 处理 HTTP 状态码
来源：http://gjl.cqqwz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://apb.ydzc1.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qcr.jinqigfzy.top

JS:   resp.ok;  resp.status
来源：http://taf.hnxiangtu.top

TS:   resp.ok;  resp.status
来源：http://mqu.chenzaomai.com

Java: resp.statusCode()
来源：http://lsi.xingfuxueyuan.xyz

Go:   resp.StatusCode
来源：http://dmt.wangdashe.top

Ruby: resp.code.to_i
来源：http://qbb.uphjek.com

C#:   (int)resp.StatusCode
来源：http://aca.feifeiyinyue.top

[L08] 并发请求多个地址
来源：http://zdg.shangyingyoupin.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://csv.shangyingyoupin.top

PHP:  curl_multi_init() 系列
来源：http://cme.ctjpmb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mmd.ydzc1.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oxr.jqgufenzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://irj.tian-w.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bds.dashuyun.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jrt.havefunace.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fdw.hywenlv.cn

================================================================================
来源：http://uom.fzhhl.top

M. 命令行 / 进程 / 环境
来源：http://trx.pycfn.com

================================================================================
来源：http://foz.meibo888.top

[M01] 读取命令行参数
来源：http://mzx.aizwys.cn

Py:   sys.argv[1:]
来源：http://gud.xuanzx.com

PHP:  $argv;  $argc;
来源：http://nta.jiagoushi.top

JS:   process.argv.slice(2)
来源：http://dio.yj202588.top

TS:   process.argv.slice(2)
来源：http://ipw.yangfankeji.com

Java: args 数组（main 方法参数）
来源：http://oio.guowangkeji.top

Go:   os.Args[1:]
来源：http://sbl.andypj.xyz

Ruby: ARGV
来源：http://jfj.ivvv.top

C#:   args 数组（Main 方法参数）
来源：http://wyn.iojbl.cn

[M02] 读取环境变量
来源：http://arb.nanxinkj.top

Py:   os.environ.get("HOME")
来源：http://lma.jianghu66.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://shv.fanxiaobao.xyz

JS:   process.env.HOME
来源：http://yfa.c1oappe.top

TS:   process.env.HOME
来源：http://gjp.chenlongwang.top

Java: System.getenv("HOME")
来源：http://dic.hongshengwenyu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sfv.xylfe.cn

Ruby: ENV["HOME"]
来源：http://bdo.hywenlv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://miy.wangdashe.top

[M03] 执行外部命令
来源：http://hqs.gogol.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gzv.sweek.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bgo.jiagoushi.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zns.jlsjyb.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gfk.yuxming.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qxi.gaohongyu789.top

Go:   exec.Command("ls", "-l").Output()
来源：http://nel.fehbvm.com

Ruby: system("ls -l");  `ls -l`
来源：http://rxc.hfpthk.cn

C#:   Process.Start("ls", "-l");
来源：http://zgs.jinqigufen.top

[M04] 获取当前工作目录
来源：http://pzz.chenjidiqi.icu

Py:   os.getcwd()
来源：http://bff.zhongyouzk.top

PHP:  getcwd();
来源：http://oox.zhongyouzk.top

JS:   process.cwd()
来源：http://dyd.hnxiangtu.top

TS:   process.cwd()
来源：http://gnm.shzxlz.cn

Java: Path.of("").toAbsolutePath()
来源：http://luf.guannengcc.top

Go:   os.Getwd()
来源：http://lrd.jlsjyb.cn

Ruby: Dir.pwd
来源：http://ffy.fktsv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zbb.sjlbkw.cn

[M05] 设置退出码
来源：http://fqy.zhaomingkeji.xyz

Py:   sys.exit(1)
来源：http://bjl.nanxinkj.top

PHP:  exit(1);
来源：http://fet.vqdsnc.cn

JS:   process.exit(1)
来源：http://xnw.c1oappe.top

TS:   process.exit(1)
来源：http://rnp.redwolf501.top

Java: System.exit(1)
来源：http://xml.jinqigfzy.top

Go:   os.Exit(1)
来源：http://dfs.feifeiyinyue.top

Ruby: exit 1
来源：http://hop.jinyuanbaomall.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ppk.vehdjk.com

[M06] 向标准错误输出
来源：http://xay.tian-w.cn

Py:   print("err", file=sys.stderr)
来源：http://oxo.birdmap.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xuo.zhoulong.xyz

JS:   console.error("err")
来源：http://gjo.jinyuanbaomall.cn

TS:   console.error("err")
来源：http://spm.52xcode.cn

Java: System.err.println("err")
来源：http://eig.jiagoushi.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rpl.meibo888.top

Ruby: warn "err"
来源：http://kon.52xcode.cn

C#:   Console.Error.WriteLine("err")
来源：http://roj.ppjwa.cn

[M07] 判断是否为主入口
来源：http://ztj.shanyushiyangkeji.top

Py:   if __name__ == "__main__":
来源：http://djr.9152youxi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bya.birdmap.top

JS:   require.main === module
来源：http://wqe.daria6918.cn

TS:   require.main === module
来源：http://pjo.feifeiyinyue.top

Java: public static void main(String[] args)
来源：http://xao.fehbvm.com

Go:   func main()
来源：http://cpw.jqgufenzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://flw.hywenlv.cn

C#:   static void Main(string[] args)
来源：http://twa.pengpengdd.cyou

[M08] 获取系统与运行时信息
来源：http://oyg.yj20258888.top

Py:   platform.system();  platform.python_version()
来源：http://uvp.hywenlv.cn

PHP:  PHP_OS;  phpversion();
来源：http://swd.ppjwa.cn

JS:   process.platform;  process.version
来源：http://jqx.sysykeji.top

TS:   process.platform;  process.version
来源：http://zlq.tarul.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pxh.zdbjq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bfi.xziqi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://poc.9152youxi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ibb.jyoumei.cn

================================================================================
来源：http://ivo.xuetiantiany.cn

N. 数据结构与算法
来源：http://lpt.pycfn.com

================================================================================
来源：http://hkz.xuanzx.com

[N01] 二分查找（有序数组）
来源：http://zad.sxryk.cn

Py:   bisect.bisect_left(arr, x)
来源：http://unz.fktsv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pxm.jlsjyb.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bpe.snrcjt.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://btz.pycfn.com

Java: Arrays.binarySearch(arr, x)
来源：http://bib.zdbjq.cn

Go:   sort.SearchInts(arr, x)
来源：http://gmo.birdmap.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://gis.sufxvd.cn

C#:   Array.BinarySearch(arr, x)
来源：http://giy.nanxuanxn.top

[N02] 排序（工程实践用内置实现）
来源：http://bby.hnqzz.top

Py:   sorted(arr);  arr.sort()
来源：http://ldj.yueranfly.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mvv.jinyuanbaomall.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xmq.ydjk.org.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mxu.dashuyun.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rkb.jyoumei.cn

Go:   slices.Sort(arr)
来源：http://zxd.haohaochexian.top


<!-- 参考信息 -->