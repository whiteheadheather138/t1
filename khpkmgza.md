代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://txk.snrcjt.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oku.iojbl.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dzo.ehwqpu.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://syx.yfazqb.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fuq.jqgfzy.top

Go:   defer f.Close()
来源：http://qck.zhiwuduotai.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kkp.zhongyouzk.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ntu.yangfankeji.com

================================================================================
来源：http://hgn.yfazqb.com

I. 正则表达式
来源：http://fol.ctjpmb.com

================================================================================
来源：http://hoy.0kj1m.cn

[I01] 判断是否匹配
来源：http://ake.andypj.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kcd.fehbvm.com

PHP:  preg_match('/\d+/', $s);
来源：http://ikf.yvedp.cn

JS:   /\d+/.test(s)
来源：http://ltu.sufxvd.cn

TS:   /\d+/.test(s)
来源：http://pxa.zhongyouzk.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qxq.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vbj.cashguo.top

Ruby: s.match?(/\d+/)
来源：http://mts.yueranfly.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://etf.xuetiantiany.cn

[I02] 提取所有匹配
来源：http://inz.hongshengwenyu.top

Py:   re.findall(r"\d+", s)
来源：http://ecb.fktsv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://amg.xylfe.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fnw.yuanzhike.top

TS:   s.match(/\d+/g)
来源：http://nsb.hnxiangtu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pmf.hesvh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ttq.c1oappe.top

Ruby: s.scan(/\d+/)
来源：http://wgu.yuanzhike.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sty.ywan-chungtsiang.top

[I03] 提取捕获分组
来源：http://kiy.sysykeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ysx.52xcode.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wyg.smart0.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tdv.aizwys.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vym.jianghu66.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://arg.zhengqikj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bky.cqqwz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nfl.hammf.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pik.hysaishi.cn

[I04] 正则替换
来源：http://ppi.jinqigfzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jyq.cqqwz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yio.hywenlv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://exl.hnqzz.top

TS:   s.replace(/\d+/g, "#")
来源：http://rmc.birdmap.top

Java: s.replaceAll("\\d+", "#")
来源：http://khu.vehdjk.com

Go:   re.ReplaceAllString(s, "#")
来源：http://pqy.xylfe.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nzo.zycfv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://oed.yuxming.cn

[I05] 按正则拆分
来源：http://uqf.zhongyouzk.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xwe.yueranfly.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uix.cucudq.cn

JS:   s.split(/\s*,\s*/)
来源：http://dgq.zhiwuduotai.top

TS:   s.split(/\s*,\s*/)
来源：http://mrd.yvedp.cn

Java: s.split("\\s*,\\s*")
来源：http://fho.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ane.ehwqpu.com

Ruby: s.split(/\s*,\s*/)
来源：http://qdo.xinyue.icu

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ixl.shuidangran.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://euy.yanxiufei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iyf.9152youxi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pfr.ppjwa.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xmw.jinghuilouyu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vox.guannengcc.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://iyr.snrcjt.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nxh.zycfv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hmk.yanxiufei.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ige.zhaomingkeji.xyz

[I07] 忽略大小写与多行模式
来源：http://xgi.fktsv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yue.gotoacloud.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zgj.yuxming.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uhm.zhixingplan.top

TS:   /error/gim
来源：http://djv.sjlbkw.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zgp.cheryme.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://eml.hcnkem.com

Ruby: s.scan(/error/i)
来源：http://klr.cucudq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xwc.zhoulong.xyz

[I08] 贪婪与非贪婪匹配
来源：http://awg.zdbjq.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jjm.yanxiufei.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rur.shzxlz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://emm.316326.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cjh.hywenlv.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lel.xuanzx.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ifv.nanxinkj.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qoz.jianghu66.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dqk.haohaochexian.top

================================================================================
来源：http://are.0kj1m.cn

J. 日期与时间
来源：http://qhg.zhiwuduotai.top

================================================================================
来源：http://ldl.hfpthk.cn

[J01] 获取当前时间
来源：http://frk.chenjidiqi.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://chi.hcnkem.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kaq.fehbvm.com

JS:   new Date();  Date.now()
来源：http://yzf.cheryme.top

TS:   new Date();  Date.now()
来源：http://ayy.hesvh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fcb.yuxming.cn

Go:   time.Now()
来源：http://tlv.fanxiaobao.xyz

Ruby: Time.now
来源：http://bpe.yongpay.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rrv.xylfe.cn

[J02] 格式化输出
来源：http://blh.yj20258888.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rgi.hysaishi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hmh.gogol.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qjk.yvedp.cn

TS:   d.toISOString()
来源：http://zse.chenlongwang.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ogd.snrcjt.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ehk.gaohongyu789.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jgu.jinghuilouyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://eeu.ehwqpu.com

[J03] 字符串解析为日期
来源：http://hen.zdbjq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ifv.nwbrower.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ivn.jinghuilouyu.cn

JS:   new Date("2024-01-02")
来源：http://rkv.chenzaomai.com

TS:   new Date("2024-01-02")
来源：http://dlf.wangdashe.top

Java: LocalDate.parse("2024-01-02")
来源：http://jos.zdbjq.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://czj.zhiwuduotai.top

Ruby: Date.parse("2024-01-02")
来源：http://qgc.zhixingplan.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nok.bjfxy.top

[J04] 时间戳与日期互转
来源：http://tvg.dianchejie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rjs.jinqigufen.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://air.hcnkem.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://caz.hnqzz.top

TS:   Math.floor(Date.now() / 1000)
来源：http://mnq.zhijiandao.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qjl.zhongyouzk.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://igi.chenlongwang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nbj.yj202588.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nun.tarul.cn

[J05] 时间加减（加 7 天）
来源：http://qfq.sjlbkw.cn

Py:   now + timedelta(days=7)
来源：http://qox.guowangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ucq.jinqigufen.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fvx.iojbl.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sir.cheryme.top

Java: LocalDate.now().plusDays(7)
来源：http://oet.yanxiufei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tap.jianghu66.top

Ruby: Time.now + 7 * 86400
来源：http://zdc.kuanghao11.cn

C#:   DateTime.Now.AddDays(7)
来源：http://uqa.xylfe.cn

[J06] 计算两时间之差
来源：http://xnp.daria6918.cn

Py:   (end - start).total_seconds()
来源：http://oax.hfpthk.cn

PHP:  $end->diff($start)->days;
来源：http://fkl.jinghuilouyu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://igy.yonumen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://krr.9152youxi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rsk.jinqigufen.top

Go:   end.Sub(start).Hours()
来源：http://zqj.cdnleiting.top

Ruby: end - start                 # 返回秒数
来源：http://dya.zhengqikj.top

C#:   (end - start).TotalSeconds
来源：http://ezm.chenjidiqi.icu

[J07] 比较两个日期
来源：http://nbc.fzhhl.top

Py:   d1 < d2;  d1 == d2
来源：http://frd.snrcjt.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yje.pycfn.com

JS:   d1.getTime() < d2.getTime()
来源：http://hsg.xuanzx.com

TS:   d1.getTime() < d2.getTime()
来源：http://cug.jianghu66.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lhe.hnxiangtu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nie.kuanghao11.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wun.52xcode.cn

C#:   d1 < d2;  d1 == d2
来源：http://wdz.mhx1999.top

[J08] 提取年月日与星期
来源：http://mlx.zhongyouzk.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bee.svipenyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oir.gogol.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pkj.yfazqb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yhl.ivvv.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://amf.316326.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fxv.ywan-chungtsiang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ica.iojbl.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fwv.yueranfly.top

[J09] 时区处理
来源：http://ftw.wangdashe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yhy.snrcjt.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tgt.cheryme.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ivr.bjfxy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bdj.cdnleiting.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://say.yj202588.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wha.smart0.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://koi.pycfn.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ewg.sysykeji.top

[J10] 取今天 / 本月第一天
来源：http://rrq.andypj.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://abm.nwbrower.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dym.sysykeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fts.vqdsnc.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gum.zhengqikj.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://aiq.andypj.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kha.chenjidiqi.icu

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://eqm.shzxlz.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eew.yj20258.top

================================================================================
来源：http://qda.fehbvm.com

K. JSON 与序列化
来源：http://hdo.zhengqikj.top

================================================================================
来源：http://ska.yj202588.top

[K01] 对象转 JSON 字符串
来源：http://tnj.hcnkem.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sbz.haohaochexian.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nni.ivvv.top

JS:   JSON.stringify(obj)
来源：http://bkb.jlsjyb.cn

TS:   JSON.stringify(obj)
来源：http://yzj.jinqigfzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ttc.9152youxi.cn

Go:   json.Marshal(obj)
来源：http://dri.pycfn.com

Ruby: obj.to_json                                     // require "json"
来源：http://ghn.tianlin.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://fkv.dashuyun.cn

[K02] JSON 字符串转对象
来源：http://ymg.ybcxt.top

Py:   json.loads(s)
来源：http://ary.hongshengwenyu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://shv.zdqjudy.top

JS:   JSON.parse(s)
来源：http://bmu.hnxiangtu.top

TS:   JSON.parse(s)
来源：http://iiz.cheryme.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ffc.uphjek.com

Go:   json.Unmarshal(data, &v)
来源：http://uok.cqqwz.cn

Ruby: JSON.parse(s)
来源：http://zue.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dpu.yj20258.top

[K03] JSON 美化输出（带缩进）
来源：http://nik.zhiwuduotai.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zbr.yj20258888.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sdb.cucudq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xjr.xuetiantiany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xuu.epnwcf.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pon.zdqjudy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lns.yuxming.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rna.hnqzz.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://skg.jinqigfzy.top

[K04] 读取 JSON 文件
来源：http://hsa.9152youxi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wkg.redwolf501.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uzo.zhoulong.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://har.haohaochexian.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lhw.ivvv.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rfp.52xcode.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nqu.chenlongwang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://gvd.shanyushiyangtech.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://myp.yuanzhike.top

[K05] 深拷贝对象
来源：http://xsx.vehdjk.com

Py:   copy.deepcopy(obj)
来源：http://hev.yfazqb.com

PHP:  unserialize(serialize($obj));
来源：http://ofl.dianchejie.cn

JS:   structuredClone(obj)
来源：http://gam.gotoacloud.top

TS:   structuredClone(obj)
来源：http://bwo.nanxuanxn.top

Java: // 手写拷贝构造，或序列化往返
来源：http://xiw.shangyingyoupin.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vgr.ppjwa.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jyv.chenzaomai.com

C#:   // 序列化往返，或自定义 Clone
来源：http://vzo.yongpay.top

[K06] 解析 URL 查询串
来源：http://cyh.ydjk.org.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://grc.quarkkingdee.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://whs.tianlin.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wmx.shzxlz.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nmj.redwolf501.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ski.guannengcc.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://knf.yuanzhike.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kwb.hammf.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://svx.chenjidiqi.icu

[K07] 进制转换
来源：http://osz.ydjk.org.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cfc.ehwqpu.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://npm.shuidangran.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cte.zhijiandao.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cck.zhiwuduotai.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://twu.snrcjt.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://csx.shuidangran.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nqw.0kj1m.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qcm.hysaishi.cn

[K08] 二进制序列化（非 JSON）
来源：http://aqq.gaohongyu789.top

Py:   pickle.dumps(obj)
来源：http://ndz.chenzaomai.com

PHP:  serialize($obj);  unserialize($s);
来源：http://bnb.jinqigufen.top

JS:   v8.serialize(obj)        // Node
来源：http://wiw.sufxvd.cn

TS:   v8.serialize(obj)        // Node
来源：http://lul.jqgufenzy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ntg.bjfxy.top

Go:   encoding/gob
来源：http://nhf.hammf.cn

Ruby: Marshal.dump(obj)
来源：http://uxg.wangshuangyany.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xnp.yj20258.top

================================================================================
来源：http://eml.ehwqpu.com

L. 网络请求
来源：http://oyt.hysaishi.cn

================================================================================
来源：http://ywx.ppjwa.cn

[L01] 发送 GET 请求
来源：http://ekb.shanyushiyangkeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jnw.jqgufenzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xsd.cdnleiting.top

JS:   await fetch(url)
来源：http://oly.xylfe.cn

TS:   await fetch(url)
来源：http://sli.fktsv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://eyh.birdmap.top

Go:   resp, err := http.Get(url)
来源：http://iuq.tianlin.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://bcw.pycfn.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://udg.quarkkingdee.top

[L02] 发送 POST JSON
来源：http://lqx.fktsv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cmh.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jfi.jyoumei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://byp.snrcjt.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://adt.xylfe.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vij.yonumen.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lka.pengpengdd.cyou

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hvd.chenzaomai.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jvi.hfpthk.cn

[L03] 设置自定义请求头
来源：http://vbt.zhoulong.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xhr.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qrg.tian-w.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jls.pycfn.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uyt.tanke756.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lfw.fengsongda.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yjl.hfpthk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://usz.quarkkingdee.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tlw.yangfankeji.com

[L04] 设置超时
来源：http://jcd.nanxuanxn.top

Py:   requests.get(url, timeout=5)
来源：http://lla.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hub.pengpengdd.cyou

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fqi.tarul.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ysy.daria6918.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://szz.haohaochexian.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mtc.316326.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wps.jqgufenzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ciz.hongshengwenyu.top

[L05] 上传文件（multipart）
来源：http://twf.nanxuanxn.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hbq.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dfl.hammf.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qov.haohaochexian.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gag.uphjek.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ihv.shzxlz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mbm.zhengqikj.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vhi.yonumen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qdb.jlsjyb.cn

[L06] 解析响应为 JSON
来源：http://sal.yfazqb.com


<!-- 参考信息 -->