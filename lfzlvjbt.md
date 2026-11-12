代发 wailian999

TS:   s.match(/\d+/g)
来源：http://lbm.hywenlv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kze.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jfg.ivvv.top

Ruby: s.scan(/\d+/)
来源：http://ahd.ctjpmb.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nsp.yongpay.top

[I03] 提取捕获分组
来源：http://psh.ydzc1.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gxg.snrcjt.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://htf.gaohongyu789.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sts.chenlongwang.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lev.bbcook.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wsk.fktsv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ixk.jqgufenzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ggu.fanxiaobao.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qdt.yuanzhike.top

[I04] 正则替换
来源：http://arj.hnqzz.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qya.sufxvd.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ben.cdnleiting.top

JS:   s.replace(/\d+/g, "#")
来源：http://fcu.pycfn.com

TS:   s.replace(/\d+/g, "#")
来源：http://slk.jyoumei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rte.zhiwuduotai.top

Go:   re.ReplaceAllString(s, "#")
来源：http://tjy.ehwqpu.com

Ruby: s.gsub(/\d+/, "#")
来源：http://zfk.andypj.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zcw.cheryme.top

[I05] 按正则拆分
来源：http://ayf.jinqigfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ibl.yueranfly.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fdz.shzxlz.cn

JS:   s.split(/\s*,\s*/)
来源：http://xmv.jlsjyb.cn

TS:   s.split(/\s*,\s*/)
来源：http://cse.yuxming.cn

Java: s.split("\\s*,\\s*")
来源：http://dnu.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xvi.haohaochexian.top

Ruby: s.split(/\s*,\s*/)
来源：http://lvr.0kj1m.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ipv.zhongyouzk.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tru.havefunace.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qin.zhengqikj.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xqc.bbcook.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xch.guannengcc.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://var.yuanzhike.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://aez.xingfuxueyuan.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tjr.pengpengdd.cyou

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zxb.haohaochexian.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://aiq.gotoacloud.top

[I07] 忽略大小写与多行模式
来源：http://tga.xuanzx.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gvv.xingfuxueyuan.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lkt.shangyingyoupin.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://btb.redwolf501.top

TS:   /error/gim
来源：http://yye.sweek.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zsb.hammf.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dug.dashuyun.cn

Ruby: s.scan(/error/i)
来源：http://lag.aibaodan.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jld.yuxming.cn

[I08] 贪婪与非贪婪匹配
来源：http://upi.zhongyouzk.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wxp.gotoacloud.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bwv.yangfankeji.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fyu.yj20258.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cxo.quarkkingdee.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://fuk.birdmap.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ykk.hysaishi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pxo.zhiwuduotai.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yku.hysaishi.cn

================================================================================
来源：http://nqa.gogol.net.cn

J. 日期与时间
来源：http://zvl.gzhubu.top

================================================================================
来源：http://cxu.52xcode.cn

[J01] 获取当前时间
来源：http://xqw.ehwqpu.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://zuy.haohaochexian.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ssg.ivvv.top

JS:   new Date();  Date.now()
来源：http://rsv.chenjidiqi.icu

TS:   new Date();  Date.now()
来源：http://zkp.svipenyu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qlq.shanyushiyangkeji.top

Go:   time.Now()
来源：http://gmb.shuidangran.top

Ruby: Time.now
来源：http://fcl.ppjwa.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ban.xinyue.icu

[J02] 格式化输出
来源：http://vzj.hysaishi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ngt.fengsongda.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hrp.sufxvd.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cjr.cdnleiting.top

TS:   d.toISOString()
来源：http://ufn.cucudq.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jsr.cqqwz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tlr.fktsv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ofh.ctjpmb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://azl.shuidangran.top

[J03] 字符串解析为日期
来源：http://ydg.ybcxt.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fqh.yvedp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://crr.yangfankeji.com

JS:   new Date("2024-01-02")
来源：http://nyx.uphjek.com

TS:   new Date("2024-01-02")
来源：http://xwl.ydjk.org.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mxl.smart0.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ujm.xuanzx.com

Ruby: Date.parse("2024-01-02")
来源：http://ynd.yvedp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://umi.shzxlz.cn

[J04] 时间戳与日期互转
来源：http://dji.hfpthk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sgb.yueranfly.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://low.jlsjyb.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vqd.aibaodan.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://quc.nanxuanxn.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eza.zhaomingkeji.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://met.sweek.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zpg.ydjk.org.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ewi.sweek.top

[J05] 时间加减（加 7 天）
来源：http://hpw.zhaomingkeji.xyz

Py:   now + timedelta(days=7)
来源：http://khr.zhengqikj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://zuv.hongshengwenyu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ted.ydzc1.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bfm.gotoacloud.top

Java: LocalDate.now().plusDays(7)
来源：http://vmy.sysykeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hxz.chenlongwang.top

Ruby: Time.now + 7 * 86400
来源：http://zhv.aibaodan.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wqt.havefunace.top

[J06] 计算两时间之差
来源：http://qaz.birdmap.top

Py:   (end - start).total_seconds()
来源：http://yui.yangfankeji.com

PHP:  $end->diff($start)->days;
来源：http://tfd.zhengqikj.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kfb.52xcode.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pkh.wangshuangyany.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bcb.chenjidiqi.icu

Go:   end.Sub(start).Hours()
来源：http://onb.hnxiangtu.top

Ruby: end - start                 # 返回秒数
来源：http://sjf.jiagoushi.top

C#:   (end - start).TotalSeconds
来源：http://xzf.yonumen.top

[J07] 比较两个日期
来源：http://sar.xuetiantiany.cn

Py:   d1 < d2;  d1 == d2
来源：http://zwm.tian-w.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nth.guowangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://spq.xylfe.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vxb.meibo888.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cxq.jinghuilouyu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oeb.zhixingplan.top

Ruby: d1 < d2;  d1 == d2
来源：http://sjf.yj20258.top

C#:   d1 < d2;  d1 == d2
来源：http://gze.feifeiyinyue.top

[J08] 提取年月日与星期
来源：http://pyk.birdmap.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rty.xinyue.icu

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wbz.ybcxt.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yil.9152youxi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://iuh.kuanghao11.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ser.bbcook.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tab.hnxiangtu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pql.snrcjt.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yum.andypj.xyz

[J09] 时区处理
来源：http://eti.shzxlz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dja.jinqigufen.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lqw.wangshuangyany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ybe.fehbvm.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gpr.iojbl.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jlh.tian-w.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://shd.yueranfly.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zbp.bbcook.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cwl.nanxuanxn.top

[J10] 取今天 / 本月第一天
来源：http://kfn.hongshengwenyu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://lmk.yfazqb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jdz.ywan-chungtsiang.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cqj.daxiang520.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bua.gaohongyu789.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://phq.hysaishi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ofg.ydzc1.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mkn.fehbvm.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vmi.gotoacloud.top

================================================================================
来源：http://beo.xuetiantiany.cn

K. JSON 与序列化
来源：http://nsd.jianghu66.top

================================================================================
来源：http://cgf.hcnkem.com

[K01] 对象转 JSON 字符串
来源：http://zmw.jqgufenzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://haq.zhaomingkeji.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vyp.redwolf501.top

JS:   JSON.stringify(obj)
来源：http://txd.cdnleiting.top

TS:   JSON.stringify(obj)
来源：http://tyn.zhoulong.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rmk.hnqzz.top

Go:   json.Marshal(obj)
来源：http://xqr.smart0.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://stx.sysykeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://mqf.zhengqikj.top

[K02] JSON 字符串转对象
来源：http://uxq.aibaodan.cn

Py:   json.loads(s)
来源：http://qpt.sufxvd.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qra.mhx1999.top

JS:   JSON.parse(s)
来源：http://asl.yj20258888.top

TS:   JSON.parse(s)
来源：http://hmd.ehwqpu.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kne.jinyuanbaomall.cn

Go:   json.Unmarshal(data, &v)
来源：http://nwg.kuanghao11.cn

Ruby: JSON.parse(s)
来源：http://tsb.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://utn.dianchejie.cn

[K03] JSON 美化输出（带缩进）
来源：http://gvm.cdnleiting.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yfi.xinyue.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ofx.hongshengwenyu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://zif.jqgfzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://aav.yanxiufei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vna.ybcxt.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xpq.daria6918.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nre.c1oappe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pju.dashuyun.cn

[K04] 读取 JSON 文件
来源：http://jhc.dianchejie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://opb.jqgufenzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://atq.yuanzhike.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lxu.xinyue.icu

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pzm.chenjidiqi.icu

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jlf.chenzaomai.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://twt.andypj.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://sks.fanxiaobao.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pcj.xuetiantiany.cn

[K05] 深拷贝对象
来源：http://tph.ydzc1.top

Py:   copy.deepcopy(obj)
来源：http://oyc.yj20258888.top

PHP:  unserialize(serialize($obj));
来源：http://scr.vehdjk.com

JS:   structuredClone(obj)
来源：http://cyq.zdbjq.cn

TS:   structuredClone(obj)
来源：http://wqx.yj20258888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://nqe.cashguo.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zyu.bjfxy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wip.haohaochexian.top

C#:   // 序列化往返，或自定义 Clone
来源：http://anr.pengpengdd.cyou

[K06] 解析 URL 查询串
来源：http://myv.aizwys.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qif.epnwcf.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gpy.nanxuanxn.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ihf.zdqjudy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://egw.yuxming.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://phd.jqgufenzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://rth.hnxiangtu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cbx.yuanzhike.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kjm.316326.xyz

[K07] 进制转换
来源：http://gqe.yj20258.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wdr.hammf.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ndf.fengsongda.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://eqb.gogol.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qfb.tanke756.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://upb.chenzaomai.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mld.zdbjq.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kah.zhijiandao.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xix.andypj.xyz

[K08] 二进制序列化（非 JSON）
来源：http://xnr.zhoulong.xyz

Py:   pickle.dumps(obj)
来源：http://kaf.sweek.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wsw.yj20258888.top

JS:   v8.serialize(obj)        // Node
来源：http://qwb.xingfuxueyuan.xyz

TS:   v8.serialize(obj)        // Node
来源：http://arr.xuetiantiany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mxi.0kj1m.cn

Go:   encoding/gob
来源：http://ytp.52xcode.cn

Ruby: Marshal.dump(obj)
来源：http://siy.meibo888.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nkj.xylfe.cn

================================================================================
来源：http://jam.xuetiantiany.cn

L. 网络请求
来源：http://uny.sxryk.cn

================================================================================
来源：http://uvd.sweek.top

[L01] 发送 GET 请求
来源：http://aov.yvedp.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qza.ppjwa.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bkg.xingfuxueyuan.xyz

JS:   await fetch(url)
来源：http://mtn.redwolf501.top

TS:   await fetch(url)
来源：http://vzn.chenlongwang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tfm.shanyushiyangtech.top

Go:   resp, err := http.Get(url)
来源：http://pvv.9152youxi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rha.0kj1m.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gxw.nwbrower.top

[L02] 发送 POST JSON
来源：http://tsw.hysaishi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ezr.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rsn.ydjk.org.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://btr.haohaochexian.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fkr.yj202588.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ztw.aizwys.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qew.hongshengwenyu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://whe.xinyue.icu

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bvg.fengsongda.top

[L03] 设置自定义请求头
来源：http://csy.zdqjudy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qdo.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://myy.hfpthk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gib.havefunace.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ovj.daxiang520.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://evx.yangfankeji.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wxs.ydzc1.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fkg.snrcjt.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oht.smart0.xyz

[L04] 设置超时
来源：http://jwx.yuxming.cn

Py:   requests.get(url, timeout=5)
来源：http://hdh.sweek.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jhu.bjfxy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wmq.feifeiyinyue.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vvt.zhixingplan.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bqj.hammf.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xwy.jianghu66.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xrm.zhengqikj.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kqe.yj20258.top

[L05] 上传文件（multipart）
来源：http://wyy.iojbl.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://htg.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://chd.shuidangran.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cxk.sysykeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vyt.shanyushiyangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mul.aizwys.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jde.cqqwz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wlc.jqgufenzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ztl.sjlbkw.cn

[L06] 解析响应为 JSON
来源：http://dwk.ehwqpu.com

Py:   resp.json()
来源：http://fxj.fengsongda.top

PHP:  json_decode($body, true);
来源：http://lkp.52xcode.cn

JS:   await resp.json()
来源：http://vcs.tanke756.top

TS:   await resp.json()
来源：http://odv.birdmap.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wgm.zhiwuduotai.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kkh.zhiwuduotai.top

Ruby: JSON.parse(resp.body)
来源：http://foh.aizwys.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hqk.xuetiantiany.cn

[L07] 处理 HTTP 状态码
来源：http://wyr.redwolf501.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hyo.jqgfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xhe.dianchejie.cn

JS:   resp.ok;  resp.status
来源：http://vig.shanyushiyangtech.top

TS:   resp.ok;  resp.status
来源：http://xkf.yangfankeji.com

Java: resp.statusCode()
来源：http://rzn.hesvh.cn

Go:   resp.StatusCode
来源：http://qgc.shangyingyoupin.top

Ruby: resp.code.to_i
来源：http://nut.c1oappe.top

C#:   (int)resp.StatusCode
来源：http://tnd.fengsongda.top

[L08] 并发请求多个地址
来源：http://itj.yonumen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ehl.redwolf501.top

PHP:  curl_multi_init() 系列
来源：http://giw.bjfxy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zzh.cqqwz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://atz.xylfe.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qmx.pycfn.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mhc.ivvv.top


<!-- 参考信息 -->