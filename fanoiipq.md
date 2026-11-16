代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hnw.dianchejie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wul.xinyue.icu

JS:   /\d+/.test(s)
来源：http://vai.dianchejie.cn

TS:   /\d+/.test(s)
来源：http://xew.zhixingplan.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nno.xuanzx.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://skj.yangfankeji.com

Ruby: s.match?(/\d+/)
来源：http://hdo.yuxming.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tzv.nwbrower.top

[I02] 提取所有匹配
来源：http://jhg.yueranfly.top

Py:   re.findall(r"\d+", s)
来源：http://zxe.wangdashe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sgz.gogol.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jnd.hcnkem.com

TS:   s.match(/\d+/g)
来源：http://kjz.jlsjyb.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ava.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hxw.cdnleiting.top

Ruby: s.scan(/\d+/)
来源：http://zbf.yuanzhike.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bff.cashguo.top

[I03] 提取捕获分组
来源：http://knn.fanxiaobao.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://has.zdbjq.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lcn.cashguo.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cer.52xcode.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vnr.yonumen.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ydr.meibo888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sqr.hfpthk.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gvk.zhoulong.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vab.xuanzx.com

[I04] 正则替换
来源：http://wkj.jlsjyb.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vfy.jinghuilouyu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bjz.iojbl.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bfc.yvedp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fqf.zhixingplan.top

Java: s.replaceAll("\\d+", "#")
来源：http://ofo.shangyingyoupin.top

Go:   re.ReplaceAllString(s, "#")
来源：http://bss.shanyushiyangtech.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vcs.gaohongyu789.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://olx.cqqwz.cn

[I05] 按正则拆分
来源：http://hlt.andypj.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://xsg.ivvv.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gom.smart0.xyz

JS:   s.split(/\s*,\s*/)
来源：http://qfg.zycfv.cn

TS:   s.split(/\s*,\s*/)
来源：http://qxx.jinqigufen.top

Java: s.split("\\s*,\\s*")
来源：http://rsz.jianghu66.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://grd.smart0.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://hol.0kj1m.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nft.dashuyun.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yte.yueranfly.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://grp.snrcjt.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vgo.tian-w.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qzw.xylfe.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ylp.yj20258888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pwe.yuxming.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mby.jyoumei.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kia.zhongyouzk.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://grs.aizwys.cn

[I07] 忽略大小写与多行模式
来源：http://oez.9152youxi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hbz.aibaodan.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dpn.sysykeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yqz.uphjek.com

TS:   /error/gim
来源：http://tlx.yj20258888.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dyj.gaohongyu789.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xej.cashguo.top

Ruby: s.scan(/error/i)
来源：http://ahh.sufxvd.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lww.tanke756.top

[I08] 贪婪与非贪婪匹配
来源：http://sbb.gogol.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ojz.kuanghao11.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nmp.nwbrower.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tnw.shuidangran.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xhc.vqdsnc.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qsl.fanxiaobao.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uam.52xcode.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nkl.ydzc1.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ngf.hnxiangtu.top

================================================================================
来源：http://yfb.xinyue.icu

J. 日期与时间
来源：http://hjb.vqdsnc.cn

================================================================================
来源：http://fgh.svipenyu.cn

[J01] 获取当前时间
来源：http://jgo.daria6918.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xvr.iojbl.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://csz.cheryme.top

JS:   new Date();  Date.now()
来源：http://lbp.hnqzz.top

TS:   new Date();  Date.now()
来源：http://sjc.svipenyu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nhr.52xcode.cn

Go:   time.Now()
来源：http://wyg.0kj1m.cn

Ruby: Time.now
来源：http://osd.hysaishi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sjy.wangshuangyany.cn

[J02] 格式化输出
来源：http://rfi.ivvv.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pmy.nanxuanxn.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ofs.jianghu66.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ihj.sjlbkw.cn

TS:   d.toISOString()
来源：http://wur.jlsjyb.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kas.iojbl.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vuo.zycfv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://znz.ivvv.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ajt.bbcook.cn

[J03] 字符串解析为日期
来源：http://iqa.bbcook.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zug.fktsv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://myh.gotoacloud.top

JS:   new Date("2024-01-02")
来源：http://qfn.nwbrower.top

TS:   new Date("2024-01-02")
来源：http://sjp.yangfankeji.com

Java: LocalDate.parse("2024-01-02")
来源：http://mpw.yj202588.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dnd.vehdjk.com

Ruby: Date.parse("2024-01-02")
来源：http://oiw.sufxvd.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hcl.chenjidiqi.icu

[J04] 时间戳与日期互转
来源：http://brp.ydjk.org.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ydy.dianchejie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ouk.shanyushiyangkeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bkx.gogol.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://uzm.hesvh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kpf.bbcook.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rhq.xuanzx.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uwg.ydzc1.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ehq.xylfe.cn

[J05] 时间加减（加 7 天）
来源：http://rsq.shanyushiyangtech.top

Py:   now + timedelta(days=7)
来源：http://djq.zhengqikj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://cuf.epnwcf.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xli.zhiwuduotai.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jmc.guowangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://neb.shangyingyoupin.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oid.ivvv.top

Ruby: Time.now + 7 * 86400
来源：http://gzs.zhijiandao.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yiz.yonumen.top

[J06] 计算两时间之差
来源：http://glw.shuidangran.top

Py:   (end - start).total_seconds()
来源：http://sgy.daria6918.cn

PHP:  $end->diff($start)->days;
来源：http://pgx.yuanzhike.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qkt.zhaomingkeji.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fie.fzhhl.top

Java: Duration.between(start, end).toSeconds()
来源：http://not.zhoulong.xyz

Go:   end.Sub(start).Hours()
来源：http://xwb.andypj.xyz

Ruby: end - start                 # 返回秒数
来源：http://khb.gogol.net.cn

C#:   (end - start).TotalSeconds
来源：http://nys.jyoumei.cn

[J07] 比较两个日期
来源：http://czl.kuanghao11.cn

Py:   d1 < d2;  d1 == d2
来源：http://tqm.tanke756.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rqd.chenlongwang.top

JS:   d1.getTime() < d2.getTime()
来源：http://wvp.shuidangran.top

TS:   d1.getTime() < d2.getTime()
来源：http://ybb.zhengqikj.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://prc.chenjidiqi.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hcy.xuetiantiany.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hjj.xuanzx.com

C#:   d1 < d2;  d1 == d2
来源：http://pjk.sjlbkw.cn

[J08] 提取年月日与星期
来源：http://uqm.xuanzx.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tkj.sysykeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://srj.hesvh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gdk.gzhubu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fff.hcnkem.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://amw.cashguo.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nth.cdnleiting.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://soj.316326.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pnw.yj20258.top

[J09] 时区处理
来源：http://ubg.pengpengdd.cyou

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://suw.dianchejie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xus.bjfxy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wky.daria6918.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ygo.havefunace.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://srn.guowangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jbc.hesvh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://osy.daxiang520.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://egn.shzxlz.cn

[J10] 取今天 / 本月第一天
来源：http://ewp.svipenyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://sds.chenzaomai.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wla.9152youxi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kgc.zhijiandao.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jod.xinyue.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kmz.gaohongyu789.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ltn.sjlbkw.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cwy.wangdashe.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rlu.chenlongwang.top

================================================================================
来源：http://ktz.wangshuangyany.cn

K. JSON 与序列化
来源：http://tyk.fzhhl.top

================================================================================
来源：http://toc.fehbvm.com

[K01] 对象转 JSON 字符串
来源：http://rha.tanke756.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iuw.0kj1m.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tvn.wangshuangyany.cn

JS:   JSON.stringify(obj)
来源：http://kuo.9152youxi.cn

TS:   JSON.stringify(obj)
来源：http://qfi.jinghuilouyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://efy.hnqzz.top

Go:   json.Marshal(obj)
来源：http://jon.zhongyouzk.top

Ruby: obj.to_json                                     // require "json"
来源：http://fvx.daxiang520.top

C#:   JsonSerializer.Serialize(obj)
来源：http://esh.zhijiandao.cn

[K02] JSON 字符串转对象
来源：http://aba.jinqigfzy.top

Py:   json.loads(s)
来源：http://zon.zhaomingkeji.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pkk.vqdsnc.cn

JS:   JSON.parse(s)
来源：http://dyh.0kj1m.cn

TS:   JSON.parse(s)
来源：http://laz.snrcjt.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://iyj.cqqwz.cn

Go:   json.Unmarshal(data, &v)
来源：http://frm.ydzc1.top

Ruby: JSON.parse(s)
来源：http://voj.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://orw.daxiang520.top

[K03] JSON 美化输出（带缩进）
来源：http://fym.hnqzz.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kqa.jqgfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wnc.gotoacloud.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ail.ydjk.org.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vpe.birdmap.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ibq.fktsv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qyr.sxryk.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vyh.pycfn.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://iby.9152youxi.cn

[K04] 读取 JSON 文件
来源：http://mzm.bjfxy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ziw.ydzc1.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zbz.hesvh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://etr.wangshuangyany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nqt.yvedp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pcn.sweek.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rpu.aizwys.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pwo.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cnm.andypj.xyz

[K05] 深拷贝对象
来源：http://kho.andypj.xyz

Py:   copy.deepcopy(obj)
来源：http://vtr.pycfn.com

PHP:  unserialize(serialize($obj));
来源：http://mnu.gzhubu.top

JS:   structuredClone(obj)
来源：http://eqv.jiagoushi.top

TS:   structuredClone(obj)
来源：http://csy.hongshengwenyu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://idz.wangdashe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xys.pengpengdd.cyou

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nak.jqgfzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://dmg.zdqjudy.top

[K06] 解析 URL 查询串
来源：http://hdr.chenlongwang.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bsm.shanyushiyangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hji.vehdjk.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ysf.jinghuilouyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gmb.feifeiyinyue.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yhx.zhixingplan.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://was.sxryk.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zgc.hcnkem.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nkq.yj20258.top

[K07] 进制转换
来源：http://mpv.316326.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pts.xuanzx.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mxn.wangdashe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lpu.yuanzhike.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nni.yueranfly.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://avd.yongpay.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://obf.yanxiufei.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yth.havefunace.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ngv.tianlin.xyz

[K08] 二进制序列化（非 JSON）
来源：http://jdq.tianlin.xyz

Py:   pickle.dumps(obj)
来源：http://wcr.cucudq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hss.bjfxy.top

JS:   v8.serialize(obj)        // Node
来源：http://dkl.nwbrower.top

TS:   v8.serialize(obj)        // Node
来源：http://ckc.sxryk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pcs.fanxiaobao.xyz

Go:   encoding/gob
来源：http://fsz.sufxvd.cn

Ruby: Marshal.dump(obj)
来源：http://vbz.yvedp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zuo.daxiang520.top

================================================================================
来源：http://gid.sysykeji.top

L. 网络请求
来源：http://tne.wangshuangyany.cn

================================================================================
来源：http://wgs.guannengcc.top

[L01] 发送 GET 请求
来源：http://xyv.ybcxt.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tnx.redwolf501.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xys.hongshengwenyu.top

JS:   await fetch(url)
来源：http://uul.ivvv.top

TS:   await fetch(url)
来源：http://meq.xuanzx.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jfo.jinyuanbaomall.cn

Go:   resp, err := http.Get(url)
来源：http://xga.gaohongyu789.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kzo.yvedp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bpa.haohaochexian.top

[L02] 发送 POST JSON
来源：http://vpd.wangdashe.top

Py:   requests.post(url, json={"a": 1})
来源：http://eic.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sef.ybcxt.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dls.yuxming.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zhg.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://eoa.zhaomingkeji.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qjv.gotoacloud.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nhm.redwolf501.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bcg.havefunace.top

[L03] 设置自定义请求头
来源：http://cwg.zhiwuduotai.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kli.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://roc.zhaomingkeji.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://chd.hongshengwenyu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ckl.yj202588.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://att.hfpthk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ahg.jqgfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://msr.snrcjt.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://szi.shanyushiyangkeji.top

[L04] 设置超时
来源：http://wqf.sysykeji.top

Py:   requests.get(url, timeout=5)
来源：http://kaj.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://udr.316326.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hfh.xuetiantiany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://onw.hcnkem.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uqv.shanyushiyangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://adq.yj20258.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wli.hnxiangtu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bmw.yuanzhike.top

[L05] 上传文件（multipart）
来源：http://kin.cheryme.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qfa.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ppy.xziqi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vyx.zhoulong.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://urm.hysaishi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qve.daxiang520.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zrg.yj20258888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://peu.tianlin.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lmc.feifeiyinyue.top

[L06] 解析响应为 JSON
来源：http://han.xuanzx.com

Py:   resp.json()
来源：http://wxx.yj20258888.top

PHP:  json_decode($body, true);
来源：http://jkr.feifeiyinyue.top

JS:   await resp.json()
来源：http://eca.yj20258.top

TS:   await resp.json()
来源：http://rdd.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ntf.gogol.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tgh.tianlin.xyz

Ruby: JSON.parse(resp.body)
来源：http://bpm.andypj.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://prj.wangshuangyany.cn

[L07] 处理 HTTP 状态码
来源：http://efj.vehdjk.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jan.hammf.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://txs.hcnkem.com

JS:   resp.ok;  resp.status
来源：http://beu.smart0.xyz


<!-- 参考信息 -->