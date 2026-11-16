代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qos.dashuyun.cn

[I03] 提取捕获分组
来源：http://bgz.xingfuxueyuan.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dqi.yueranfly.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ikb.0kj1m.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tqd.yj202588.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://igz.sweek.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://udh.xinyue.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iyo.zdbjq.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kiw.ppjwa.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cte.0kj1m.cn

[I04] 正则替换
来源：http://yff.hammf.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kjk.c1oappe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vnv.chenjidiqi.icu

JS:   s.replace(/\d+/g, "#")
来源：http://tyk.epnwcf.com

TS:   s.replace(/\d+/g, "#")
来源：http://wup.epnwcf.com

Java: s.replaceAll("\\d+", "#")
来源：http://tad.zhoulong.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://tkq.vqdsnc.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cnk.ybcxt.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tcj.cdnleiting.top

[I05] 按正则拆分
来源：http://zro.yanxiufei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lzc.zhiwuduotai.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yte.jinqigufen.top

JS:   s.split(/\s*,\s*/)
来源：http://lqt.yonumen.top

TS:   s.split(/\s*,\s*/)
来源：http://lyx.smart0.xyz

Java: s.split("\\s*,\\s*")
来源：http://vvg.xinyue.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://igw.birdmap.top

Ruby: s.split(/\s*,\s*/)
来源：http://ibp.jiagoushi.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cca.sxryk.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ufh.tianlin.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://umv.chenjidiqi.icu

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iry.dashuyun.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://csy.jianghu66.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://emp.hammf.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mmc.ctjpmb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://skk.zdbjq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://esr.cdnleiting.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hxl.hammf.cn

[I07] 忽略大小写与多行模式
来源：http://xah.fengsongda.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fsi.yongpay.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qdv.gzhubu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://smd.dianchejie.cn

TS:   /error/gim
来源：http://etv.jyoumei.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jrt.gotoacloud.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ziz.ppjwa.cn

Ruby: s.scan(/error/i)
来源：http://jjs.jqgfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hsa.guannengcc.top

[I08] 贪婪与非贪婪匹配
来源：http://vif.hysaishi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wiv.zhaomingkeji.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yop.svipenyu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ons.wangdashe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://srw.hywenlv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dvu.yueranfly.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://env.ivvv.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blb.jqgufenzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://swv.fktsv.cn

================================================================================
来源：http://tsb.andypj.xyz

J. 日期与时间
来源：http://shy.mhx1999.top

================================================================================
来源：http://wxw.svipenyu.cn

[J01] 获取当前时间
来源：http://krn.hammf.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gwy.aizwys.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nzn.jiagoushi.top

JS:   new Date();  Date.now()
来源：http://edu.yangfankeji.com

TS:   new Date();  Date.now()
来源：http://mxz.hnxiangtu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ptb.ywan-chungtsiang.top

Go:   time.Now()
来源：http://scx.hongshengwenyu.top

Ruby: Time.now
来源：http://tsm.ywan-chungtsiang.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://alb.cashguo.top

[J02] 格式化输出
来源：http://erh.52xcode.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sjt.smart0.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vgp.sweek.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bdh.cheryme.top

TS:   d.toISOString()
来源：http://xnr.cheryme.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bqo.gogol.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://svu.zhoulong.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kmo.hcnkem.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iwf.hammf.cn

[J03] 字符串解析为日期
来源：http://fyx.ydjk.org.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kbz.nanxinkj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ptg.yj20258888.top

JS:   new Date("2024-01-02")
来源：http://jiq.hcnkem.com

TS:   new Date("2024-01-02")
来源：http://cnf.zhengqikj.top

Java: LocalDate.parse("2024-01-02")
来源：http://gdu.fehbvm.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://raa.mhx1999.top

Ruby: Date.parse("2024-01-02")
来源：http://sma.zhengqikj.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vut.gogol.net.cn

[J04] 时间戳与日期互转
来源：http://uuc.yj20258.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://inc.guannengcc.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://goo.vehdjk.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pwk.zhongyouzk.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wne.wangdashe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jvc.jqgufenzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qlz.fengsongda.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kkb.gotoacloud.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ffs.jinyuanbaomall.cn

[J05] 时间加减（加 7 天）
来源：http://jwy.shanyushiyangtech.top

Py:   now + timedelta(days=7)
来源：http://nxf.9152youxi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fqm.jinghuilouyu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mjp.dianchejie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zka.vqdsnc.cn

Java: LocalDate.now().plusDays(7)
来源：http://nth.hammf.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gbf.xuetiantiany.cn

Ruby: Time.now + 7 * 86400
来源：http://ubb.jinqigfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://ezd.jqgufenzy.top

[J06] 计算两时间之差
来源：http://bum.dianchejie.cn

Py:   (end - start).total_seconds()
来源：http://nyu.bbcook.cn

PHP:  $end->diff($start)->days;
来源：http://ayp.xziqi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dki.cucudq.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ybl.wangshuangyany.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hxc.sufxvd.cn

Go:   end.Sub(start).Hours()
来源：http://xmp.chenzaomai.com

Ruby: end - start                 # 返回秒数
来源：http://khx.fengsongda.top

C#:   (end - start).TotalSeconds
来源：http://zmp.aizwys.cn

[J07] 比较两个日期
来源：http://bzk.yj20258888.top

Py:   d1 < d2;  d1 == d2
来源：http://dqv.yuxming.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tbg.tanke756.top

JS:   d1.getTime() < d2.getTime()
来源：http://bsv.shuidangran.top

TS:   d1.getTime() < d2.getTime()
来源：http://fir.chenjidiqi.icu

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cqv.gogol.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ulp.yj20258888.top

Ruby: d1 < d2;  d1 == d2
来源：http://jjb.pengpengdd.cyou

C#:   d1 < d2;  d1 == d2
来源：http://qey.yonumen.top

[J08] 提取年月日与星期
来源：http://tfk.fehbvm.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ihl.gzhubu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mno.chenlongwang.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xfn.chenjidiqi.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kqz.316326.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://erp.jianghu66.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lwg.nanxinkj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aby.hywenlv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kwm.nanxuanxn.top

[J09] 时区处理
来源：http://rmv.shzxlz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cbm.shanyushiyangtech.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vog.smart0.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pef.chenjidiqi.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kax.xylfe.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zeo.vehdjk.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vdc.ydzc1.top

Ruby: Time.now.getlocal("+08:00")
来源：http://viv.wangshuangyany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kwj.dashuyun.cn

[J10] 取今天 / 本月第一天
来源：http://ekv.yvedp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gko.yuanzhike.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yja.yj20258888.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hqk.pengpengdd.cyou

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://axv.havefunace.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jwe.ywan-chungtsiang.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ihq.redwolf501.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://iej.hfpthk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uxt.zdbjq.cn

================================================================================
来源：http://iqs.jqgufenzy.top

K. JSON 与序列化
来源：http://lrw.52xcode.cn

================================================================================
来源：http://edb.yueranfly.top

[K01] 对象转 JSON 字符串
来源：http://vzq.wangshuangyany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vnt.jinqigfzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hqm.52xcode.cn

JS:   JSON.stringify(obj)
来源：http://dsa.vqdsnc.cn

TS:   JSON.stringify(obj)
来源：http://vko.jianghu66.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xmi.iojbl.cn

Go:   json.Marshal(obj)
来源：http://axo.cdnleiting.top

Ruby: obj.to_json                                     // require "json"
来源：http://nrl.shanyushiyangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zhy.hongshengwenyu.top

[K02] JSON 字符串转对象
来源：http://lwr.yonumen.top

Py:   json.loads(s)
来源：http://cym.hywenlv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gsx.dashuyun.cn

JS:   JSON.parse(s)
来源：http://yxo.xuanzx.com

TS:   JSON.parse(s)
来源：http://thx.uphjek.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://eid.yuanzhike.top

Go:   json.Unmarshal(data, &v)
来源：http://fjj.jianghu66.top

Ruby: JSON.parse(s)
来源：http://wih.hesvh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wnh.nanxinkj.top

[K03] JSON 美化输出（带缩进）
来源：http://twr.xuetiantiany.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rsp.hnqzz.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://shz.nwbrower.top

JS:   JSON.stringify(obj, null, 2)
来源：http://aia.fengsongda.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xcx.fanxiaobao.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mkf.nwbrower.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rpw.hfpthk.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bfm.guowangkeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vrc.havefunace.top

[K04] 读取 JSON 文件
来源：http://joj.xuetiantiany.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uvd.fanxiaobao.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lpl.iojbl.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://etc.wangdashe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xod.sysykeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hls.fengsongda.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gne.ctjpmb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://wff.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rzg.c1oappe.top

[K05] 深拷贝对象
来源：http://veo.daxiang520.top

Py:   copy.deepcopy(obj)
来源：http://fmf.yueranfly.top

PHP:  unserialize(serialize($obj));
来源：http://mbm.xylfe.cn

JS:   structuredClone(obj)
来源：http://nnm.jianghu66.top

TS:   structuredClone(obj)
来源：http://vxe.shanyushiyangtech.top

Java: // 手写拷贝构造，或序列化往返
来源：http://sxt.shuidangran.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gkb.snrcjt.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dlv.xuetiantiany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ybn.ydjk.org.cn

[K06] 解析 URL 查询串
来源：http://shy.shanyushiyangtech.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gyv.chenzaomai.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xsx.pengpengdd.cyou

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nxl.ydjk.org.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eee.chenzaomai.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lhz.ppjwa.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jqu.sweek.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vdm.sufxvd.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ebg.yongpay.top

[K07] 进制转换
来源：http://hot.ybcxt.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gzh.epnwcf.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://unx.xylfe.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://egg.cqqwz.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uaj.yuxming.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vwy.yueranfly.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nyy.hysaishi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vpd.sysykeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bae.xinyue.icu

[K08] 二进制序列化（非 JSON）
来源：http://pon.hywenlv.cn

Py:   pickle.dumps(obj)
来源：http://aqr.yfazqb.com

PHP:  serialize($obj);  unserialize($s);
来源：http://eln.cdnleiting.top

JS:   v8.serialize(obj)        // Node
来源：http://yky.zhiwuduotai.top

TS:   v8.serialize(obj)        // Node
来源：http://yto.jqgfzy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bnh.fanxiaobao.xyz

Go:   encoding/gob
来源：http://llj.smart0.xyz

Ruby: Marshal.dump(obj)
来源：http://djy.aizwys.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jse.gzhubu.top

================================================================================
来源：http://erv.iojbl.cn

L. 网络请求
来源：http://vwi.fzhhl.top

================================================================================
来源：http://zcy.xziqi.cn

[L01] 发送 GET 请求
来源：http://upd.hesvh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nrq.yueranfly.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wgo.cheryme.top

JS:   await fetch(url)
来源：http://uno.zdqjudy.top

TS:   await fetch(url)
来源：http://dhh.yj202588.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://aqb.daxiang520.top

Go:   resp, err := http.Get(url)
来源：http://nle.zhiwuduotai.top

Ruby: Net::HTTP.get(URI(url))
来源：http://cbn.jiagoushi.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vtb.shanyushiyangtech.top

[L02] 发送 POST JSON
来源：http://lxc.hongshengwenyu.top

Py:   requests.post(url, json={"a": 1})
来源：http://zts.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tqf.hfpthk.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vee.daxiang520.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gva.bjfxy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uko.meibo888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://grt.jinqigfzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ydy.fengsongda.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lrj.9152youxi.cn

[L03] 设置自定义请求头
来源：http://dwo.jinqigufen.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wkm.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hhx.hnxiangtu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dai.daxiang520.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rkg.jianghu66.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kva.tian-w.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://msb.xylfe.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hgl.shangyingyoupin.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cjm.gotoacloud.top

[L04] 设置超时
来源：http://rns.yj202588.top

Py:   requests.get(url, timeout=5)
来源：http://lvb.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://icr.yueranfly.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bpa.wangshuangyany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ztb.fehbvm.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dve.jiagoushi.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hqe.zhaomingkeji.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lxg.jinghuilouyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mbe.hnqzz.top

[L05] 上传文件（multipart）
来源：http://nbi.ivvv.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uzx.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hka.52xcode.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mpq.gogol.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nhx.hnqzz.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lxd.snrcjt.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lfq.fengsongda.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qyq.jlsjyb.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ptz.yanxiufei.cn

[L06] 解析响应为 JSON
来源：http://zne.xuanzx.com

Py:   resp.json()
来源：http://fxr.52xcode.cn

PHP:  json_decode($body, true);
来源：http://rjh.hfpthk.cn

JS:   await resp.json()
来源：http://bku.aizwys.cn

TS:   await resp.json()
来源：http://dqr.sjlbkw.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ebg.ctjpmb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://evr.chenzaomai.com

Ruby: JSON.parse(resp.body)
来源：http://uvh.jqgufenzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vjv.aibaodan.cn

[L07] 处理 HTTP 状态码
来源：http://ixg.kuanghao11.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://swz.kuanghao11.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://eaf.ppjwa.cn

JS:   resp.ok;  resp.status
来源：http://hdc.svipenyu.cn

TS:   resp.ok;  resp.status
来源：http://psx.yanxiufei.cn

Java: resp.statusCode()
来源：http://qax.nanxuanxn.top

Go:   resp.StatusCode
来源：http://ovb.yj20258888.top

Ruby: resp.code.to_i
来源：http://npk.0kj1m.cn

C#:   (int)resp.StatusCode
来源：http://zxo.xuanzx.com

[L08] 并发请求多个地址
来源：http://fab.316326.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gxg.shzxlz.cn

PHP:  curl_multi_init() 系列
来源：http://mrv.jlsjyb.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://txz.cheryme.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qlf.yfazqb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://odn.epnwcf.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hqs.nwbrower.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nif.haohaochexian.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fvw.fehbvm.com

================================================================================
来源：http://pws.kuanghao11.cn

M. 命令行 / 进程 / 环境
来源：http://rmv.aibaodan.cn


<!-- 参考信息 -->