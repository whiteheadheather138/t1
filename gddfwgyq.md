代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://gti.316326.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://cch.zdbjq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://soz.sufxvd.cn

[I05] 按正则拆分
来源：http://ost.yuxming.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xcg.zhoulong.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tbj.tianlin.xyz

JS:   s.split(/\s*,\s*/)
来源：http://hln.jiagoushi.top

TS:   s.split(/\s*,\s*/)
来源：http://hie.zdqjudy.top

Java: s.split("\\s*,\\s*")
来源：http://afs.shanyushiyangtech.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://syv.vqdsnc.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lli.zhijiandao.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rko.haohaochexian.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bfa.shangyingyoupin.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vjc.jiagoushi.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uzs.shzxlz.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sju.yuxming.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ihq.mhx1999.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ltp.wangshuangyany.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pun.fengsongda.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fkl.hongshengwenyu.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://myr.hammf.cn

[I07] 忽略大小写与多行模式
来源：http://erm.xuetiantiany.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://amg.hywenlv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bjr.yangfankeji.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bsa.mhx1999.top

TS:   /error/gim
来源：http://gjv.iojbl.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cll.wangshuangyany.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://otq.zhengqikj.top

Ruby: s.scan(/error/i)
来源：http://sse.cashguo.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lly.sysykeji.top

[I08] 贪婪与非贪婪匹配
来源：http://xqw.aibaodan.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ivy.daxiang520.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tfc.yueranfly.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qzv.zdqjudy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dko.cdnleiting.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://vtt.cashguo.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://moo.sjlbkw.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wyb.tarul.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nzt.andypj.xyz

================================================================================
来源：http://reo.0kj1m.cn

J. 日期与时间
来源：http://jfs.vqdsnc.cn

================================================================================
来源：http://vui.jlsjyb.cn

[J01] 获取当前时间
来源：http://cme.pengpengdd.cyou

Py:   datetime.now();  datetime.now(UTC)
来源：http://nfk.nanxinkj.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ukw.uphjek.com

JS:   new Date();  Date.now()
来源：http://qwd.zhijiandao.cn

TS:   new Date();  Date.now()
来源：http://ajg.ppjwa.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lry.zdqjudy.top

Go:   time.Now()
来源：http://cke.tianlin.xyz

Ruby: Time.now
来源：http://dhf.gotoacloud.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gav.ppjwa.cn

[J02] 格式化输出
来源：http://gcm.guowangkeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lhs.yuanzhike.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mcy.fehbvm.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://miy.hesvh.cn

TS:   d.toISOString()
来源：http://rej.yuxming.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dxj.sjlbkw.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zqu.yongpay.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xhu.haohaochexian.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zlb.yonumen.top

[J03] 字符串解析为日期
来源：http://ywd.uphjek.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cfn.hywenlv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nmq.0kj1m.cn

JS:   new Date("2024-01-02")
来源：http://bgy.ivvv.top

TS:   new Date("2024-01-02")
来源：http://uug.kuanghao11.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cpf.tanke756.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qtk.cucudq.cn

Ruby: Date.parse("2024-01-02")
来源：http://wtt.tian-w.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ild.yvedp.cn

[J04] 时间戳与日期互转
来源：http://nwu.yj202588.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dty.yueranfly.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bej.haohaochexian.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://awb.hysaishi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://isz.daria6918.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xoj.jqgfzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://olz.fengsongda.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jqx.yuanzhike.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://spb.quarkkingdee.top

[J05] 时间加减（加 7 天）
来源：http://pgj.xuanzx.com

Py:   now + timedelta(days=7)
来源：http://ibf.zhijiandao.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rjy.nwbrower.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nwm.ydjk.org.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ede.jlsjyb.cn

Java: LocalDate.now().plusDays(7)
来源：http://lhh.chenlongwang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dky.ivvv.top

Ruby: Time.now + 7 * 86400
来源：http://dan.jiagoushi.top

C#:   DateTime.Now.AddDays(7)
来源：http://esl.hammf.cn

[J06] 计算两时间之差
来源：http://iba.ydzc1.top

Py:   (end - start).total_seconds()
来源：http://jdp.wangshuangyany.cn

PHP:  $end->diff($start)->days;
来源：http://ecm.uphjek.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://djk.kuanghao11.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jgt.yuxming.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hql.yanxiufei.cn

Go:   end.Sub(start).Hours()
来源：http://svd.aibaodan.cn

Ruby: end - start                 # 返回秒数
来源：http://qve.aibaodan.cn

C#:   (end - start).TotalSeconds
来源：http://mpx.yvedp.cn

[J07] 比较两个日期
来源：http://onm.haohaochexian.top

Py:   d1 < d2;  d1 == d2
来源：http://tyx.jyoumei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jyp.sysykeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://ikx.ybcxt.top

TS:   d1.getTime() < d2.getTime()
来源：http://wid.bjfxy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ugx.c1oappe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hzf.shanyushiyangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://hxq.9152youxi.cn

C#:   d1 < d2;  d1 == d2
来源：http://nkm.zhiwuduotai.top

[J08] 提取年月日与星期
来源：http://omo.hongshengwenyu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xlx.yvedp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://npg.fktsv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gmv.jlsjyb.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lrp.nwbrower.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tgl.epnwcf.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pso.cashguo.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qgt.cucudq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nta.shzxlz.cn

[J09] 时区处理
来源：http://pjq.xinyue.icu

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ebh.gogol.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lmc.zhijiandao.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xns.ctjpmb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xcp.yanxiufei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xbf.zhiwuduotai.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zcw.yueranfly.top

Ruby: Time.now.getlocal("+08:00")
来源：http://syn.jqgufenzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://egn.yvedp.cn

[J10] 取今天 / 本月第一天
来源：http://xzb.pycfn.com

Py:   date.today();  date.today().replace(day=1)
来源：http://acv.316326.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kcp.fzhhl.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vyx.ppjwa.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jxf.xingfuxueyuan.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ckw.zhiwuduotai.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xqc.xinyue.icu

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hwp.0kj1m.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zfc.sjlbkw.cn

================================================================================
来源：http://gza.zhoulong.xyz

K. JSON 与序列化
来源：http://tme.mhx1999.top

================================================================================
来源：http://ldb.birdmap.top

[K01] 对象转 JSON 字符串
来源：http://stl.ehwqpu.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tjo.zdbjq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ugq.hongshengwenyu.top

JS:   JSON.stringify(obj)
来源：http://xhw.sysykeji.top

TS:   JSON.stringify(obj)
来源：http://zae.aizwys.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bjo.jlsjyb.cn

Go:   json.Marshal(obj)
来源：http://sdi.hammf.cn

Ruby: obj.to_json                                     // require "json"
来源：http://esc.nanxuanxn.top

C#:   JsonSerializer.Serialize(obj)
来源：http://wpz.jqgfzy.top

[K02] JSON 字符串转对象
来源：http://nep.feifeiyinyue.top

Py:   json.loads(s)
来源：http://sxx.0kj1m.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ebn.jyoumei.cn

JS:   JSON.parse(s)
来源：http://hjh.ppjwa.cn

TS:   JSON.parse(s)
来源：http://npb.sysykeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wns.jinghuilouyu.cn

Go:   json.Unmarshal(data, &v)
来源：http://vlx.hcnkem.com

Ruby: JSON.parse(s)
来源：http://hnm.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jel.sxryk.cn

[K03] JSON 美化输出（带缩进）
来源：http://xzi.ppjwa.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gig.jyoumei.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xsv.yj20258888.top

JS:   JSON.stringify(obj, null, 2)
来源：http://sty.cucudq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kms.ywan-chungtsiang.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vpy.tianlin.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pwy.zhaomingkeji.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://awf.daxiang520.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jyn.xziqi.cn

[K04] 读取 JSON 文件
来源：http://zip.yfazqb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lvs.cucudq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://imx.fzhhl.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tts.jlsjyb.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bof.dianchejie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://czm.zdbjq.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://trh.ehwqpu.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://bhn.jqgufenzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jay.fktsv.cn

[K05] 深拷贝对象
来源：http://ajq.tarul.cn

Py:   copy.deepcopy(obj)
来源：http://kyj.chenlongwang.top

PHP:  unserialize(serialize($obj));
来源：http://zgk.fzhhl.top

JS:   structuredClone(obj)
来源：http://xap.snrcjt.cn

TS:   structuredClone(obj)
来源：http://fnw.meibo888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://knr.xylfe.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nac.bbcook.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://beo.shanyushiyangtech.top

C#:   // 序列化往返，或自定义 Clone
来源：http://pup.wangdashe.top

[K06] 解析 URL 查询串
来源：http://flg.guowangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dzx.zycfv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ywr.nanxuanxn.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://brc.aibaodan.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hdl.yanxiufei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lvz.svipenyu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fuj.gzhubu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lcx.xuetiantiany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tjb.feifeiyinyue.top

[K07] 进制转换
来源：http://jbu.wangdashe.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xwa.jinqigufen.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lou.vqdsnc.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nya.nanxinkj.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cvw.pycfn.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yvl.bbcook.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ytj.316326.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fld.hysaishi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dtg.fanxiaobao.xyz

[K08] 二进制序列化（非 JSON）
来源：http://cls.meibo888.top

Py:   pickle.dumps(obj)
来源：http://tyx.bjfxy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://urd.jinyuanbaomall.cn

JS:   v8.serialize(obj)        // Node
来源：http://yps.ydzc1.top

TS:   v8.serialize(obj)        // Node
来源：http://ypy.gogol.net.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pty.jqgufenzy.top

Go:   encoding/gob
来源：http://hee.yj20258888.top

Ruby: Marshal.dump(obj)
来源：http://pia.yanxiufei.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rbj.gogol.net.cn

================================================================================
来源：http://yic.sweek.top

L. 网络请求
来源：http://bld.shuidangran.top

================================================================================
来源：http://lfz.sxryk.cn

[L01] 发送 GET 请求
来源：http://hln.iojbl.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vhr.xuetiantiany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qmd.vehdjk.com

JS:   await fetch(url)
来源：http://iuu.jinqigfzy.top

TS:   await fetch(url)
来源：http://zlp.jiagoushi.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gix.yfazqb.com

Go:   resp, err := http.Get(url)
来源：http://lkw.nanxuanxn.top

Ruby: Net::HTTP.get(URI(url))
来源：http://gql.nanxuanxn.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oog.kuanghao11.cn

[L02] 发送 POST JSON
来源：http://wsh.yvedp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ovr.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tpu.sjlbkw.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tfe.zycfv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ypf.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://njj.jinyuanbaomall.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qik.yueranfly.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mhf.xylfe.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eys.yueranfly.top

[L03] 设置自定义请求头
来源：http://zgk.ydzc1.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ewl.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://clp.aizwys.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gvp.bbcook.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dxb.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qnf.jinqigufen.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pqs.jqgufenzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zgq.jinghuilouyu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://coj.tianlin.xyz

[L04] 设置超时
来源：http://arq.jinqigufen.top

Py:   requests.get(url, timeout=5)
来源：http://nio.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bah.aibaodan.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kdu.hysaishi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sjn.birdmap.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wsq.sxryk.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jly.jinyuanbaomall.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://srw.fengsongda.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qqh.jiagoushi.top

[L05] 上传文件（multipart）
来源：http://saj.dashuyun.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vhh.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://avy.dashuyun.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rsm.zdbjq.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://swl.zdbjq.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mno.quarkkingdee.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sra.yongpay.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qol.sxryk.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dkm.yfazqb.com

[L06] 解析响应为 JSON
来源：http://try.316326.xyz

Py:   resp.json()
来源：http://lgu.guannengcc.top

PHP:  json_decode($body, true);
来源：http://lsh.svipenyu.cn

JS:   await resp.json()
来源：http://zvr.fktsv.cn

TS:   await resp.json()
来源：http://ueo.yanxiufei.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ejr.hnqzz.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hfb.nanxuanxn.top

Ruby: JSON.parse(resp.body)
来源：http://ors.vehdjk.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zzk.hesvh.cn

[L07] 处理 HTTP 状态码
来源：http://zxu.zdbjq.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://evd.xuanzx.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fzz.yueranfly.top

JS:   resp.ok;  resp.status
来源：http://yfw.chenjidiqi.icu

TS:   resp.ok;  resp.status
来源：http://xva.yfazqb.com

Java: resp.statusCode()
来源：http://oiw.nanxinkj.top

Go:   resp.StatusCode
来源：http://hus.fktsv.cn

Ruby: resp.code.to_i
来源：http://fru.quarkkingdee.top

C#:   (int)resp.StatusCode
来源：http://gsi.yj20258888.top

[L08] 并发请求多个地址
来源：http://uwb.hongshengwenyu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bgd.zhoulong.xyz

PHP:  curl_multi_init() 系列
来源：http://baw.ydzc1.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zcz.svipenyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tfa.wangdashe.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cbf.sufxvd.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eve.pengpengdd.cyou

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sic.hfpthk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://usi.jianghu66.top

================================================================================
来源：http://hvc.316326.xyz

M. 命令行 / 进程 / 环境
来源：http://fbr.yvedp.cn

================================================================================
来源：http://cwa.ivvv.top

[M01] 读取命令行参数
来源：http://cky.uphjek.com

Py:   sys.argv[1:]
来源：http://gxx.zdbjq.cn

PHP:  $argv;  $argc;
来源：http://xrd.jinghuilouyu.cn

JS:   process.argv.slice(2)
来源：http://rwo.tanke756.top

TS:   process.argv.slice(2)
来源：http://til.sufxvd.cn

Java: args 数组（main 方法参数）
来源：http://yvv.tarul.cn

Go:   os.Args[1:]
来源：http://ubf.jiagoushi.top

Ruby: ARGV
来源：http://wnb.hnqzz.top

C#:   args 数组（Main 方法参数）
来源：http://jol.aizwys.cn

[M02] 读取环境变量
来源：http://bua.dashuyun.cn

Py:   os.environ.get("HOME")
来源：http://gen.havefunace.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nvb.fengsongda.top

JS:   process.env.HOME
来源：http://iyx.havefunace.top

TS:   process.env.HOME
来源：http://jfh.ppjwa.cn

Java: System.getenv("HOME")
来源：http://txy.havefunace.top


<!-- 参考信息 -->