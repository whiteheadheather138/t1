代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qrq.guannengcc.top

JS:   s.replace(/\d+/g, "#")
来源：http://vgn.zhiwuduotai.top

TS:   s.replace(/\d+/g, "#")
来源：http://jla.jqgufenzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://wfu.yonumen.top

Go:   re.ReplaceAllString(s, "#")
来源：http://lqf.hywenlv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qdc.kuanghao11.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://emx.hfpthk.cn

[I05] 按正则拆分
来源：http://gmc.shuidangran.top

Py:   re.split(r"\s*,\s*", s)
来源：http://irc.yj20258.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xsu.hcnkem.com

JS:   s.split(/\s*,\s*/)
来源：http://xzl.birdmap.top

TS:   s.split(/\s*,\s*/)
来源：http://klq.cqqwz.cn

Java: s.split("\\s*,\\s*")
来源：http://rka.chenzaomai.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lvo.yangfankeji.com

Ruby: s.split(/\s*,\s*/)
来源：http://fmp.gzhubu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mvm.mhx1999.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pee.jinyuanbaomall.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://udy.xylfe.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mds.xingfuxueyuan.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vox.fehbvm.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fwj.hcnkem.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://egl.zhaomingkeji.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://aop.bbcook.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yro.shuidangran.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vbo.52xcode.cn

[I07] 忽略大小写与多行模式
来源：http://wme.fengsongda.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bmg.ppjwa.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gqa.havefunace.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hkd.yueranfly.top

TS:   /error/gim
来源：http://ztq.kuanghao11.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bwn.bbcook.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fui.zdbjq.cn

Ruby: s.scan(/error/i)
来源：http://nsa.daxiang520.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fgv.sxryk.cn

[I08] 贪婪与非贪婪匹配
来源：http://dxj.haohaochexian.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lra.sxryk.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bas.0kj1m.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fgm.jiagoushi.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oeb.zycfv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kuu.zhaomingkeji.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tww.xziqi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lgk.hnxiangtu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hic.wangdashe.top

================================================================================
来源：http://axr.shuidangran.top

J. 日期与时间
来源：http://qcm.fanxiaobao.xyz

================================================================================
来源：http://sks.yj202588.top

[J01] 获取当前时间
来源：http://qpv.haohaochexian.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://aag.xuetiantiany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ofs.daria6918.cn

JS:   new Date();  Date.now()
来源：http://yzw.ybcxt.top

TS:   new Date();  Date.now()
来源：http://ksw.cdnleiting.top

Java: LocalDateTime.now();  Instant.now()
来源：http://aez.zhoulong.xyz

Go:   time.Now()
来源：http://cqk.smart0.xyz

Ruby: Time.now
来源：http://cop.cheryme.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://stb.c1oappe.top

[J02] 格式化输出
来源：http://yns.dashuyun.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dpa.jqgfzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kwv.tanke756.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ihr.hywenlv.cn

TS:   d.toISOString()
来源：http://alx.zhixingplan.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xpa.chenlongwang.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fbh.gaohongyu789.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fkr.gaohongyu789.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yhf.bjfxy.top

[J03] 字符串解析为日期
来源：http://owu.hnxiangtu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vmk.vqdsnc.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hsi.haohaochexian.top

JS:   new Date("2024-01-02")
来源：http://ofd.jqgfzy.top

TS:   new Date("2024-01-02")
来源：http://pyp.hesvh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://itc.c1oappe.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dzf.jqgufenzy.top

Ruby: Date.parse("2024-01-02")
来源：http://hfw.ehwqpu.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mmn.yueranfly.top

[J04] 时间戳与日期互转
来源：http://rru.jiagoushi.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kjo.52xcode.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vde.ivvv.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uqz.daria6918.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ldl.ivvv.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dzl.tarul.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://miz.sxryk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pif.jyoumei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ruh.svipenyu.cn

[J05] 时间加减（加 7 天）
来源：http://kon.quarkkingdee.top

Py:   now + timedelta(days=7)
来源：http://ppk.birdmap.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://iju.hnqzz.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wtk.fktsv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ccl.andypj.xyz

Java: LocalDate.now().plusDays(7)
来源：http://zaw.sufxvd.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bec.yj20258888.top

Ruby: Time.now + 7 * 86400
来源：http://qud.jiagoushi.top

C#:   DateTime.Now.AddDays(7)
来源：http://axo.shanyushiyangkeji.top

[J06] 计算两时间之差
来源：http://btk.yongpay.top

Py:   (end - start).total_seconds()
来源：http://qwm.shangyingyoupin.top

PHP:  $end->diff($start)->days;
来源：http://pfs.daria6918.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cte.cheryme.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kse.gotoacloud.top

Java: Duration.between(start, end).toSeconds()
来源：http://lyy.sysykeji.top

Go:   end.Sub(start).Hours()
来源：http://bjd.cashguo.top

Ruby: end - start                 # 返回秒数
来源：http://hng.sufxvd.cn

C#:   (end - start).TotalSeconds
来源：http://uyw.epnwcf.com

[J07] 比较两个日期
来源：http://jth.kuanghao11.cn

Py:   d1 < d2;  d1 == d2
来源：http://qel.vehdjk.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wpb.hesvh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ihd.havefunace.top

TS:   d1.getTime() < d2.getTime()
来源：http://twp.wangshuangyany.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tpk.cashguo.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pse.nanxinkj.top

Ruby: d1 < d2;  d1 == d2
来源：http://fkc.epnwcf.com

C#:   d1 < d2;  d1 == d2
来源：http://iiw.hfpthk.cn

[J08] 提取年月日与星期
来源：http://jii.ywan-chungtsiang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xks.zhongyouzk.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sbp.fanxiaobao.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pqn.jinghuilouyu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gbg.hesvh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kcv.cdnleiting.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://abt.gotoacloud.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zye.havefunace.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zml.zdqjudy.top

[J09] 时区处理
来源：http://wbl.dashuyun.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gek.havefunace.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ogu.zhijiandao.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://egk.yanxiufei.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vbc.jianghu66.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://aft.guowangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://von.sysykeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://syv.xuetiantiany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fem.zdbjq.cn

[J10] 取今天 / 本月第一天
来源：http://lom.birdmap.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rsn.havefunace.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iff.bbcook.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xhh.hysaishi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ynn.52xcode.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uhr.yongpay.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://imq.zhixingplan.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oug.jinghuilouyu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nxt.sweek.top

================================================================================
来源：http://lxt.0kj1m.cn

K. JSON 与序列化
来源：http://ivl.chenzaomai.com

================================================================================
来源：http://rjd.sxryk.cn

[K01] 对象转 JSON 字符串
来源：http://thv.yangfankeji.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gsi.pengpengdd.cyou

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zpl.ydzc1.top

JS:   JSON.stringify(obj)
来源：http://wyv.nanxinkj.top

TS:   JSON.stringify(obj)
来源：http://zsb.redwolf501.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tqh.cdnleiting.top

Go:   json.Marshal(obj)
来源：http://gys.guannengcc.top

Ruby: obj.to_json                                     // require "json"
来源：http://sbd.bjfxy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ccw.316326.xyz

[K02] JSON 字符串转对象
来源：http://jvy.cqqwz.cn

Py:   json.loads(s)
来源：http://fiw.kuanghao11.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jec.uphjek.com

JS:   JSON.parse(s)
来源：http://pad.sysykeji.top

TS:   JSON.parse(s)
来源：http://uzv.sysykeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ucz.yangfankeji.com

Go:   json.Unmarshal(data, &v)
来源：http://uta.dashuyun.cn

Ruby: JSON.parse(s)
来源：http://aej.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cwv.yj20258.top

[K03] JSON 美化输出（带缩进）
来源：http://lkp.nwbrower.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lce.yuxming.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tlj.pycfn.com

JS:   JSON.stringify(obj, null, 2)
来源：http://ass.cqqwz.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gyh.cheryme.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ehf.xziqi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oqd.smart0.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://wlc.jinghuilouyu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://icv.xinyue.icu

[K04] 读取 JSON 文件
来源：http://zbw.fktsv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://edb.zhongyouzk.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://egk.fktsv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hio.shuidangran.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kaw.hnxiangtu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://glp.gaohongyu789.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ogv.vehdjk.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://sda.jiagoushi.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xyr.xziqi.cn

[K05] 深拷贝对象
来源：http://guy.dianchejie.cn

Py:   copy.deepcopy(obj)
来源：http://mnp.redwolf501.top

PHP:  unserialize(serialize($obj));
来源：http://cbf.nanxuanxn.top

JS:   structuredClone(obj)
来源：http://lsy.yuanzhike.top

TS:   structuredClone(obj)
来源：http://dgq.ppjwa.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kmr.shuidangran.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xqh.jinqigufen.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lvi.zdbjq.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nmz.xuanzx.com

[K06] 解析 URL 查询串
来源：http://icj.aizwys.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fov.daria6918.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zhh.xingfuxueyuan.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nbk.birdmap.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://olr.ywan-chungtsiang.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nxz.ydjk.org.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://lgl.sjlbkw.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qwo.haohaochexian.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://geb.jinqigufen.top

[K07] 进制转换
来源：http://hgp.redwolf501.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xpr.jinghuilouyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gfo.shanyushiyangkeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xcm.ydjk.org.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hiu.zhoulong.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gbz.yj202588.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uyf.sweek.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rrw.wangdashe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ifg.havefunace.top

[K08] 二进制序列化（非 JSON）
来源：http://cfr.pengpengdd.cyou

Py:   pickle.dumps(obj)
来源：http://ezb.zhoulong.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://jbb.shanyushiyangtech.top

JS:   v8.serialize(obj)        // Node
来源：http://dgk.zhaomingkeji.xyz

TS:   v8.serialize(obj)        // Node
来源：http://hpt.yj20258.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://glh.sysykeji.top

Go:   encoding/gob
来源：http://bbh.yj20258.top

Ruby: Marshal.dump(obj)
来源：http://cbk.pengpengdd.cyou

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://eny.yanxiufei.cn

================================================================================
来源：http://bbj.cqqwz.cn

L. 网络请求
来源：http://bhv.sysykeji.top

================================================================================
来源：http://qjf.zhongyouzk.top

[L01] 发送 GET 请求
来源：http://jsa.sxryk.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ana.nwbrower.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zlv.zdbjq.cn

JS:   await fetch(url)
来源：http://wdf.nanxuanxn.top

TS:   await fetch(url)
来源：http://wwm.shangyingyoupin.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dtz.hfpthk.cn

Go:   resp, err := http.Get(url)
来源：http://cfj.gotoacloud.top

Ruby: Net::HTTP.get(URI(url))
来源：http://plg.jiagoushi.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wuz.ctjpmb.com

[L02] 发送 POST JSON
来源：http://ytw.hysaishi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://grb.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lnw.zycfv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xxi.yuanzhike.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zsy.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zby.mhx1999.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zcc.vehdjk.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tcf.hfpthk.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lub.bbcook.cn

[L03] 设置自定义请求头
来源：http://aix.gaohongyu789.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xza.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ztu.ivvv.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://muz.cheryme.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ehf.jinqigufen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mak.daxiang520.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://via.9152youxi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mwc.fehbvm.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hlx.dashuyun.cn

[L04] 设置超时
来源：http://vui.hongshengwenyu.top

Py:   requests.get(url, timeout=5)
来源：http://yqa.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://eov.zdbjq.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kpy.fehbvm.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://voc.cdnleiting.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://obx.cqqwz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hbl.vehdjk.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qsj.yanxiufei.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jfa.tianlin.xyz

[L05] 上传文件（multipart）
来源：http://uub.nanxinkj.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uhz.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uqo.tarul.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hyw.yj20258.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://she.ppjwa.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://buz.jqgufenzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lbf.zycfv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mbb.jinqigufen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hvj.haohaochexian.top

[L06] 解析响应为 JSON
来源：http://les.xingfuxueyuan.xyz

Py:   resp.json()
来源：http://ocm.ctjpmb.com

PHP:  json_decode($body, true);
来源：http://uuo.aizwys.cn

JS:   await resp.json()
来源：http://yex.tianlin.xyz

TS:   await resp.json()
来源：http://jum.shzxlz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nyz.nwbrower.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://buo.fanxiaobao.xyz

Ruby: JSON.parse(resp.body)
来源：http://xwr.ppjwa.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://egd.zycfv.cn

[L07] 处理 HTTP 状态码
来源：http://iur.guowangkeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mwq.aibaodan.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yto.hesvh.cn

JS:   resp.ok;  resp.status
来源：http://xto.xziqi.cn

TS:   resp.ok;  resp.status
来源：http://sda.fzhhl.top

Java: resp.statusCode()
来源：http://cof.shanyushiyangkeji.top

Go:   resp.StatusCode
来源：http://dlj.sufxvd.cn

Ruby: resp.code.to_i
来源：http://bop.nanxuanxn.top

C#:   (int)resp.StatusCode
来源：http://ptw.snrcjt.cn

[L08] 并发请求多个地址
来源：http://dhk.zdbjq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ldi.smart0.xyz

PHP:  curl_multi_init() 系列
来源：http://gsg.fzhhl.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fcp.yongpay.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ubc.zdbjq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tyv.hywenlv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vff.yuxming.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wyw.guannengcc.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vqa.zhiwuduotai.top

================================================================================
来源：http://gcy.nanxuanxn.top

M. 命令行 / 进程 / 环境
来源：http://hjf.hfpthk.cn

================================================================================
来源：http://aow.0kj1m.cn

[M01] 读取命令行参数
来源：http://cbj.hnqzz.top

Py:   sys.argv[1:]
来源：http://fzv.shanyushiyangkeji.top

PHP:  $argv;  $argc;
来源：http://xfr.jiagoushi.top

JS:   process.argv.slice(2)
来源：http://bhu.yuxming.cn

TS:   process.argv.slice(2)
来源：http://tgj.jianghu66.top

Java: args 数组（main 方法参数）
来源：http://ewg.xziqi.cn

Go:   os.Args[1:]
来源：http://deb.yuanzhike.top

Ruby: ARGV
来源：http://fci.jinyuanbaomall.cn

C#:   args 数组（Main 方法参数）
来源：http://anv.mhx1999.top

[M02] 读取环境变量
来源：http://qga.fehbvm.com

Py:   os.environ.get("HOME")
来源：http://azo.jianghu66.top


<!-- 参考信息 -->