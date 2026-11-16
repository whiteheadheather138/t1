代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tlb.gotoacloud.top

JS:   s.replace(/\d+/g, "#")
来源：http://qny.chenzaomai.com

TS:   s.replace(/\d+/g, "#")
来源：http://haz.zhixingplan.top

Java: s.replaceAll("\\d+", "#")
来源：http://dhk.yueranfly.top

Go:   re.ReplaceAllString(s, "#")
来源：http://kyu.nwbrower.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kxl.yueranfly.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dar.shanyushiyangtech.top

[I05] 按正则拆分
来源：http://lkc.cdnleiting.top

Py:   re.split(r"\s*,\s*", s)
来源：http://zkd.jqgufenzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ogl.daria6918.cn

JS:   s.split(/\s*,\s*/)
来源：http://yxj.haohaochexian.top

TS:   s.split(/\s*,\s*/)
来源：http://jcp.yuxming.cn

Java: s.split("\\s*,\\s*")
来源：http://epj.havefunace.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://brf.cucudq.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ncg.redwolf501.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nov.snrcjt.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vkn.52xcode.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wmj.birdmap.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wnr.gzhubu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wrn.zhoulong.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zph.chenzaomai.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kxq.gaohongyu789.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ddj.jinghuilouyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mii.ivvv.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ynp.chenzaomai.com

[I07] 忽略大小写与多行模式
来源：http://lzo.zhengqikj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pxa.havefunace.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wla.zhaomingkeji.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://edd.shanyushiyangkeji.top

TS:   /error/gim
来源：http://rwq.smart0.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hxw.cdnleiting.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xbf.guannengcc.top

Ruby: s.scan(/error/i)
来源：http://njn.haohaochexian.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mgj.jinghuilouyu.cn

[I08] 贪婪与非贪婪匹配
来源：http://izt.hnxiangtu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hwd.shanyushiyangkeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jwf.zhixingplan.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ezs.ydzc1.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://djy.zdbjq.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://die.smart0.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qtk.daxiang520.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gyn.gaohongyu789.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jqh.quarkkingdee.top

================================================================================
来源：http://rbq.xingfuxueyuan.xyz

J. 日期与时间
来源：http://unz.xinyue.icu

================================================================================
来源：http://pwm.cashguo.top

[J01] 获取当前时间
来源：http://jdb.hnxiangtu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://wte.hywenlv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oqb.nanxuanxn.top

JS:   new Date();  Date.now()
来源：http://anj.316326.xyz

TS:   new Date();  Date.now()
来源：http://wsm.xylfe.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ynq.xuetiantiany.cn

Go:   time.Now()
来源：http://nnz.zhoulong.xyz

Ruby: Time.now
来源：http://kcn.iojbl.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://aea.gogol.net.cn

[J02] 格式化输出
来源：http://ubz.wangdashe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wde.cdnleiting.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nhy.yuxming.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vob.zhongyouzk.top

TS:   d.toISOString()
来源：http://ggm.xylfe.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rzv.snrcjt.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zqf.ppjwa.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jcy.jinghuilouyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://igm.uphjek.com

[J03] 字符串解析为日期
来源：http://vbo.shanyushiyangtech.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rwu.vqdsnc.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://enf.zhoulong.xyz

JS:   new Date("2024-01-02")
来源：http://sew.yuxming.cn

TS:   new Date("2024-01-02")
来源：http://jcs.xuanzx.com

Java: LocalDate.parse("2024-01-02")
来源：http://jnu.zhixingplan.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uwo.yfazqb.com

Ruby: Date.parse("2024-01-02")
来源：http://lnb.zhixingplan.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jur.xuanzx.com

[J04] 时间戳与日期互转
来源：http://ibf.smart0.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jil.zhiwuduotai.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zmd.gogol.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://npa.xziqi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pgi.jinyuanbaomall.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xkb.dashuyun.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fgv.yuxming.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qdy.yuanzhike.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yzr.jinqigufen.top

[J05] 时间加减（加 7 天）
来源：http://smp.zdqjudy.top

Py:   now + timedelta(days=7)
来源：http://ejo.tanke756.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://hfk.kuanghao11.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kyd.tian-w.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lcz.tianlin.xyz

Java: LocalDate.now().plusDays(7)
来源：http://tcx.quarkkingdee.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fer.ppjwa.cn

Ruby: Time.now + 7 * 86400
来源：http://vqd.jinqigfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://yjt.dashuyun.cn

[J06] 计算两时间之差
来源：http://zxk.nwbrower.top

Py:   (end - start).total_seconds()
来源：http://jfp.yvedp.cn

PHP:  $end->diff($start)->days;
来源：http://rpw.ywan-chungtsiang.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://liv.pycfn.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xek.zhaomingkeji.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://wto.iojbl.cn

Go:   end.Sub(start).Hours()
来源：http://war.zhijiandao.cn

Ruby: end - start                 # 返回秒数
来源：http://kow.cucudq.cn

C#:   (end - start).TotalSeconds
来源：http://ain.ydjk.org.cn

[J07] 比较两个日期
来源：http://bei.yueranfly.top

Py:   d1 < d2;  d1 == d2
来源：http://mix.hysaishi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://avu.zycfv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ywp.ctjpmb.com

TS:   d1.getTime() < d2.getTime()
来源：http://rax.cucudq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yid.fktsv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bop.zhiwuduotai.top

Ruby: d1 < d2;  d1 == d2
来源：http://cda.xylfe.cn

C#:   d1 < d2;  d1 == d2
来源：http://pqf.zdbjq.cn

[J08] 提取年月日与星期
来源：http://sff.zdbjq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://oik.mhx1999.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pbc.daxiang520.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ohw.andypj.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ryp.nanxuanxn.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cym.sufxvd.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://aww.vqdsnc.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://byc.zhixingplan.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uhd.meibo888.top

[J09] 时区处理
来源：http://xsc.yangfankeji.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jth.ywan-chungtsiang.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://khi.hongshengwenyu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://srr.jinqigufen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pcx.epnwcf.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ofe.zhoulong.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ggl.bbcook.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://elt.ybcxt.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://knx.tianlin.xyz

[J10] 取今天 / 本月第一天
来源：http://hvm.hcnkem.com

Py:   date.today();  date.today().replace(day=1)
来源：http://ivs.yonumen.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xfh.aizwys.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ffi.ybcxt.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bvs.ydjk.org.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sjp.cdnleiting.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://psv.shanyushiyangtech.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://emc.316326.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oek.cdnleiting.top

================================================================================
来源：http://vze.guowangkeji.top

K. JSON 与序列化
来源：http://cvj.sjlbkw.cn

================================================================================
来源：http://yum.snrcjt.cn

[K01] 对象转 JSON 字符串
来源：http://qfw.ivvv.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wlt.hnxiangtu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://thz.ppjwa.cn

JS:   JSON.stringify(obj)
来源：http://vhs.pengpengdd.cyou

TS:   JSON.stringify(obj)
来源：http://fub.chenlongwang.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jrz.yangfankeji.com

Go:   json.Marshal(obj)
来源：http://hjs.cqqwz.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dqo.zdbjq.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qzc.pycfn.com

[K02] JSON 字符串转对象
来源：http://kog.guowangkeji.top

Py:   json.loads(s)
来源：http://xry.fehbvm.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ckg.0kj1m.cn

JS:   JSON.parse(s)
来源：http://hjx.birdmap.top

TS:   JSON.parse(s)
来源：http://sjj.nwbrower.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nyo.0kj1m.cn

Go:   json.Unmarshal(data, &v)
来源：http://tey.wangdashe.top

Ruby: JSON.parse(s)
来源：http://gdj.pycfn.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tfu.hnqzz.top

[K03] JSON 美化输出（带缩进）
来源：http://ylm.ydjk.org.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xzp.jqgfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tcb.fengsongda.top

JS:   JSON.stringify(obj, null, 2)
来源：http://uwq.bjfxy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://uas.wangshuangyany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jqf.hammf.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oor.tianlin.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://uhc.yfazqb.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ylo.havefunace.top

[K04] 读取 JSON 文件
来源：http://gme.yanxiufei.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://aqp.ybcxt.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://esx.0kj1m.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hju.zhaomingkeji.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jho.guowangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jae.nwbrower.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gnw.havefunace.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://fov.ywan-chungtsiang.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hnq.svipenyu.cn

[K05] 深拷贝对象
来源：http://hha.zdqjudy.top

Py:   copy.deepcopy(obj)
来源：http://zra.uphjek.com

PHP:  unserialize(serialize($obj));
来源：http://yzz.redwolf501.top

JS:   structuredClone(obj)
来源：http://pjp.fanxiaobao.xyz

TS:   structuredClone(obj)
来源：http://rwe.cheryme.top

Java: // 手写拷贝构造，或序列化往返
来源：http://cjf.havefunace.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://eqc.jyoumei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cqk.chenjidiqi.icu

C#:   // 序列化往返，或自定义 Clone
来源：http://dbp.316326.xyz

[K06] 解析 URL 查询串
来源：http://bbs.havefunace.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bjn.jiagoushi.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uih.xingfuxueyuan.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cwq.meibo888.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tye.ivvv.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zrt.yueranfly.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ppc.chenzaomai.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://guj.ybcxt.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wnu.jianghu66.top

[K07] 进制转换
来源：http://bzc.jlsjyb.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kgz.fzhhl.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qle.zhongyouzk.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ksw.pengpengdd.cyou

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gaw.hongshengwenyu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xvg.hongshengwenyu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ucx.gzhubu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ydo.jyoumei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://owy.jianghu66.top

[K08] 二进制序列化（非 JSON）
来源：http://glj.cucudq.cn

Py:   pickle.dumps(obj)
来源：http://rte.feifeiyinyue.top

PHP:  serialize($obj);  unserialize($s);
来源：http://mkz.fengsongda.top

JS:   v8.serialize(obj)        // Node
来源：http://aec.jinyuanbaomall.cn

TS:   v8.serialize(obj)        // Node
来源：http://kei.feifeiyinyue.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uqc.ppjwa.cn

Go:   encoding/gob
来源：http://vaa.gotoacloud.top

Ruby: Marshal.dump(obj)
来源：http://dhm.ctjpmb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wcd.wangshuangyany.cn

================================================================================
来源：http://nas.jiagoushi.top

L. 网络请求
来源：http://mnt.hongshengwenyu.top

================================================================================
来源：http://lcc.jianghu66.top

[L01] 发送 GET 请求
来源：http://ofe.chenzaomai.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xpp.havefunace.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ovz.yangfankeji.com

JS:   await fetch(url)
来源：http://eoc.zhongyouzk.top

TS:   await fetch(url)
来源：http://bjk.nanxinkj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://syo.dianchejie.cn

Go:   resp, err := http.Get(url)
来源：http://pqv.ydjk.org.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://oak.guowangkeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://giq.jinqigfzy.top

[L02] 发送 POST JSON
来源：http://rbp.wangshuangyany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bac.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jue.zhiwuduotai.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iff.bjfxy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uhg.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zxq.aibaodan.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nux.chenzaomai.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kcj.hfpthk.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://phl.xziqi.cn

[L03] 设置自定义请求头
来源：http://pim.ivvv.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://opb.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oid.yuanzhike.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gfr.cucudq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lsa.wangdashe.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ihw.cucudq.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rvn.xziqi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ryw.fzhhl.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wwv.c1oappe.top

[L04] 设置超时
来源：http://xen.hnqzz.top

Py:   requests.get(url, timeout=5)
来源：http://dhf.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uns.feifeiyinyue.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://etm.yfazqb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gly.chenjidiqi.icu

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://knv.chenjidiqi.icu

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yhy.hongshengwenyu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://khu.xinyue.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lru.nwbrower.top

[L05] 上传文件（multipart）
来源：http://nnh.cqqwz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gpj.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rdm.zhijiandao.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vba.hongshengwenyu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://efu.fehbvm.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fll.cashguo.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fgy.pengpengdd.cyou

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tvc.yueranfly.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://swd.xuetiantiany.cn

[L06] 解析响应为 JSON
来源：http://wwv.cdnleiting.top

Py:   resp.json()
来源：http://hrr.zhixingplan.top

PHP:  json_decode($body, true);
来源：http://srh.pycfn.com

JS:   await resp.json()
来源：http://gzi.nanxuanxn.top

TS:   await resp.json()
来源：http://bez.9152youxi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yie.cucudq.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xjz.iojbl.cn

Ruby: JSON.parse(resp.body)
来源：http://tgc.yj202588.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://svo.fengsongda.top

[L07] 处理 HTTP 状态码
来源：http://bix.daxiang520.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://swy.wangshuangyany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fbw.shanyushiyangtech.top

JS:   resp.ok;  resp.status
来源：http://rmi.cqqwz.cn

TS:   resp.ok;  resp.status
来源：http://wri.quarkkingdee.top

Java: resp.statusCode()
来源：http://ibj.gzhubu.top

Go:   resp.StatusCode
来源：http://gfl.0kj1m.cn

Ruby: resp.code.to_i
来源：http://mee.haohaochexian.top

C#:   (int)resp.StatusCode
来源：http://row.yfazqb.com

[L08] 并发请求多个地址
来源：http://lbc.snrcjt.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rtw.epnwcf.com

PHP:  curl_multi_init() 系列
来源：http://rmq.ywan-chungtsiang.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gac.tarul.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://skx.chenjidiqi.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://grw.hywenlv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tzi.shanyushiyangtech.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dei.gzhubu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kdk.daria6918.cn

================================================================================
来源：http://xrs.jyoumei.cn

M. 命令行 / 进程 / 环境
来源：http://zvs.vehdjk.com

================================================================================
来源：http://yyw.quarkkingdee.top

[M01] 读取命令行参数
来源：http://cdk.kuanghao11.cn

Py:   sys.argv[1:]
来源：http://jqr.xylfe.cn

PHP:  $argv;  $argc;
来源：http://xrk.yuanzhike.top

JS:   process.argv.slice(2)
来源：http://bdg.redwolf501.top

TS:   process.argv.slice(2)
来源：http://hgg.c1oappe.top

Java: args 数组（main 方法参数）
来源：http://tao.fanxiaobao.xyz

Go:   os.Args[1:]
来源：http://gwz.hnqzz.top

Ruby: ARGV
来源：http://gio.redwolf501.top

C#:   args 数组（Main 方法参数）
来源：http://tdp.gogol.net.cn

[M02] 读取环境变量
来源：http://biq.birdmap.top

Py:   os.environ.get("HOME")
来源：http://oam.pengpengdd.cyou


<!-- 参考信息 -->