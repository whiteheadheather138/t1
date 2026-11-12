代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xry.zdbjq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ebe.hfpthk.cn

JS:   /\d+/.test(s)
来源：http://jow.sxryk.cn

TS:   /\d+/.test(s)
来源：http://cnd.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zyp.shangyingyoupin.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://elp.zhijiandao.cn

Ruby: s.match?(/\d+/)
来源：http://xzr.zhijiandao.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vha.jinyuanbaomall.cn

[I02] 提取所有匹配
来源：http://efd.fzhhl.top

Py:   re.findall(r"\d+", s)
来源：http://qbe.svipenyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rfe.meibo888.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tag.dianchejie.cn

TS:   s.match(/\d+/g)
来源：http://pwf.zhijiandao.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kql.wangdashe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tov.aizwys.cn

Ruby: s.scan(/\d+/)
来源：http://djz.xuanzx.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mtv.haohaochexian.top

[I03] 提取捕获分组
来源：http://lhe.kuanghao11.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://aah.chenlongwang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zdd.wangshuangyany.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ndv.aibaodan.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://egq.chenzaomai.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wqo.smart0.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://avn.jinqigfzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kvp.uphjek.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hyj.smart0.xyz

[I04] 正则替换
来源：http://xct.nanxinkj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://wru.pycfn.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dbu.shangyingyoupin.top

JS:   s.replace(/\d+/g, "#")
来源：http://cyy.jiagoushi.top

TS:   s.replace(/\d+/g, "#")
来源：http://nkk.hammf.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jlc.epnwcf.com

Go:   re.ReplaceAllString(s, "#")
来源：http://tql.tanke756.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qjw.aizwys.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tas.epnwcf.com

[I05] 按正则拆分
来源：http://gkj.havefunace.top

Py:   re.split(r"\s*,\s*", s)
来源：http://dwb.vqdsnc.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hyo.jlsjyb.cn

JS:   s.split(/\s*,\s*/)
来源：http://zow.shanyushiyangkeji.top

TS:   s.split(/\s*,\s*/)
来源：http://hid.cqqwz.cn

Java: s.split("\\s*,\\s*")
来源：http://bly.bbcook.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bsy.daria6918.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hyh.zhongyouzk.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wbp.shuidangran.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uqh.cdnleiting.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ger.fktsv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://giu.hywenlv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kjq.nwbrower.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zdx.yanxiufei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ton.nanxuanxn.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qcg.dashuyun.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mkm.zhongyouzk.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lty.nanxinkj.top

[I07] 忽略大小写与多行模式
来源：http://rpw.gzhubu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iih.jlsjyb.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mkl.epnwcf.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://juq.gogol.net.cn

TS:   /error/gim
来源：http://rdm.aibaodan.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lfp.hesvh.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kms.vqdsnc.cn

Ruby: s.scan(/error/i)
来源：http://fss.jinqigfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mwe.xuetiantiany.cn

[I08] 贪婪与非贪婪匹配
来源：http://mna.vqdsnc.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bmq.dashuyun.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hyw.zhengqikj.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kbb.hnxiangtu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lwl.hysaishi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fix.jyoumei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://epq.xingfuxueyuan.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yvg.jqgufenzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bpq.yj20258.top

================================================================================
来源：http://rhh.tian-w.cn

J. 日期与时间
来源：http://ocm.jqgfzy.top

================================================================================
来源：http://wtj.yanxiufei.cn

[J01] 获取当前时间
来源：http://ngn.cqqwz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ddc.svipenyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cuh.sxryk.cn

JS:   new Date();  Date.now()
来源：http://mrh.zycfv.cn

TS:   new Date();  Date.now()
来源：http://ypd.wangdashe.top

Java: LocalDateTime.now();  Instant.now()
来源：http://bmi.meibo888.top

Go:   time.Now()
来源：http://rnh.chenzaomai.com

Ruby: Time.now
来源：http://fnu.yuanzhike.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cqz.pengpengdd.cyou

[J02] 格式化输出
来源：http://hzz.52xcode.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://enw.kuanghao11.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bbt.smart0.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jzw.yj20258888.top

TS:   d.toISOString()
来源：http://vca.ydjk.org.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uds.daxiang520.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://aog.aibaodan.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ebr.nanxinkj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iiz.ywan-chungtsiang.top

[J03] 字符串解析为日期
来源：http://ejp.zdqjudy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vvt.hysaishi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ypl.hfpthk.cn

JS:   new Date("2024-01-02")
来源：http://cpf.hongshengwenyu.top

TS:   new Date("2024-01-02")
来源：http://sae.yvedp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dzk.yj20258888.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://azb.haohaochexian.top

Ruby: Date.parse("2024-01-02")
来源：http://heu.wangshuangyany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://egp.fanxiaobao.xyz

[J04] 时间戳与日期互转
来源：http://zyc.gogol.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xus.xylfe.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bhk.haohaochexian.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nuk.gaohongyu789.top

TS:   Math.floor(Date.now() / 1000)
来源：http://obu.gzhubu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bte.guannengcc.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wfb.jinqigufen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qjo.0kj1m.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uaq.sufxvd.cn

[J05] 时间加减（加 7 天）
来源：http://dbc.chenjidiqi.icu

Py:   now + timedelta(days=7)
来源：http://cgo.tianlin.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://kgy.vqdsnc.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qay.shanyushiyangkeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://adv.nanxinkj.top

Java: LocalDate.now().plusDays(7)
来源：http://lou.jqgufenzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jnq.jinqigfzy.top

Ruby: Time.now + 7 * 86400
来源：http://rss.hammf.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ryw.pycfn.com

[J06] 计算两时间之差
来源：http://nve.yj20258.top

Py:   (end - start).total_seconds()
来源：http://fdd.gotoacloud.top

PHP:  $end->diff($start)->days;
来源：http://dzh.jinqigufen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gsi.ydzc1.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://owq.sjlbkw.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vix.gogol.net.cn

Go:   end.Sub(start).Hours()
来源：http://vky.xuanzx.com

Ruby: end - start                 # 返回秒数
来源：http://edh.birdmap.top

C#:   (end - start).TotalSeconds
来源：http://bja.mhx1999.top

[J07] 比较两个日期
来源：http://vrj.jinghuilouyu.cn

Py:   d1 < d2;  d1 == d2
来源：http://aei.dashuyun.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ghf.jinyuanbaomall.cn

JS:   d1.getTime() < d2.getTime()
来源：http://oun.shuidangran.top

TS:   d1.getTime() < d2.getTime()
来源：http://ewc.ehwqpu.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rrc.birdmap.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://saa.redwolf501.top

Ruby: d1 < d2;  d1 == d2
来源：http://uvy.zhoulong.xyz

C#:   d1 < d2;  d1 == d2
来源：http://zlv.tianlin.xyz

[J08] 提取年月日与星期
来源：http://leb.xingfuxueyuan.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hsz.uphjek.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lif.aibaodan.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bch.yvedp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wyi.zhongyouzk.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vtt.yj202588.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wct.birdmap.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vhp.redwolf501.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qkb.ivvv.top

[J09] 时区处理
来源：http://hjj.cdnleiting.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zcp.316326.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mzg.redwolf501.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tzw.zhaomingkeji.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rfz.yuxming.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mhc.chenjidiqi.icu

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uvo.guannengcc.top

Ruby: Time.now.getlocal("+08:00")
来源：http://suk.316326.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bvm.zhijiandao.cn

[J10] 取今天 / 本月第一天
来源：http://rbt.jqgufenzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://bga.hysaishi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vho.iojbl.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wgz.zdqjudy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://egh.xylfe.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bty.zhaomingkeji.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mdq.yj202588.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ver.tianlin.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bmg.tarul.cn

================================================================================
来源：http://xkq.jlsjyb.cn

K. JSON 与序列化
来源：http://dmg.vehdjk.com

================================================================================
来源：http://zlo.52xcode.cn

[K01] 对象转 JSON 字符串
来源：http://ett.316326.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bpz.uphjek.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://frj.sufxvd.cn

JS:   JSON.stringify(obj)
来源：http://mmj.sjlbkw.cn

TS:   JSON.stringify(obj)
来源：http://gkr.cheryme.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gwh.ywan-chungtsiang.top

Go:   json.Marshal(obj)
来源：http://icr.0kj1m.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bhy.tarul.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://smk.zhongyouzk.top

[K02] JSON 字符串转对象
来源：http://dvr.52xcode.cn

Py:   json.loads(s)
来源：http://sic.zycfv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pcj.ydjk.org.cn

JS:   JSON.parse(s)
来源：http://byd.snrcjt.cn

TS:   JSON.parse(s)
来源：http://agk.chenzaomai.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lxc.zhongyouzk.top

Go:   json.Unmarshal(data, &v)
来源：http://san.bjfxy.top

Ruby: JSON.parse(s)
来源：http://qyy.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://osj.hongshengwenyu.top

[K03] JSON 美化输出（带缩进）
来源：http://zod.c1oappe.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sgn.bjfxy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jaf.hongshengwenyu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://lxz.hongshengwenyu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://qfs.chenjidiqi.icu

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cvi.haohaochexian.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ztl.wangdashe.top

Ruby: JSON.pretty_generate(obj)
来源：http://jlp.yj20258888.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pxo.shanyushiyangkeji.top

[K04] 读取 JSON 文件
来源：http://yto.epnwcf.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xxg.gotoacloud.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wgg.dashuyun.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://son.daria6918.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wzv.ydzc1.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zem.jiagoushi.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rjv.xinyue.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://siq.hesvh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uhj.kuanghao11.cn

[K05] 深拷贝对象
来源：http://zum.hcnkem.com

Py:   copy.deepcopy(obj)
来源：http://mme.fengsongda.top

PHP:  unserialize(serialize($obj));
来源：http://kje.jianghu66.top

JS:   structuredClone(obj)
来源：http://lyb.jqgufenzy.top

TS:   structuredClone(obj)
来源：http://jcv.guannengcc.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mni.jlsjyb.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pgm.zhijiandao.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://awp.tanke756.top

C#:   // 序列化往返，或自定义 Clone
来源：http://wqd.fengsongda.top

[K06] 解析 URL 查询串
来源：http://nhq.daxiang520.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://slr.zycfv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pzp.sjlbkw.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uzp.bjfxy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jhl.jinghuilouyu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wvy.guannengcc.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jsr.gogol.net.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://toj.hammf.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gpc.c1oappe.top

[K07] 进制转换
来源：http://fge.xingfuxueyuan.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rxc.ctjpmb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mch.52xcode.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hcg.yonumen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yjs.cqqwz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wyz.jinqigfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bfa.pengpengdd.cyou

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rpd.shuidangran.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zzd.yj20258888.top

[K08] 二进制序列化（非 JSON）
来源：http://fgp.pycfn.com

Py:   pickle.dumps(obj)
来源：http://tvo.birdmap.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wsa.smart0.xyz

JS:   v8.serialize(obj)        // Node
来源：http://sze.cdnleiting.top

TS:   v8.serialize(obj)        // Node
来源：http://hzt.jiagoushi.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rfm.guowangkeji.top

Go:   encoding/gob
来源：http://xcn.tian-w.cn

Ruby: Marshal.dump(obj)
来源：http://dnn.fzhhl.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://exa.ivvv.top

================================================================================
来源：http://ksf.xziqi.cn

L. 网络请求
来源：http://nex.jinghuilouyu.cn

================================================================================
来源：http://txz.xziqi.cn

[L01] 发送 GET 请求
来源：http://lgf.fktsv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://snl.gogol.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rjw.bbcook.cn

JS:   await fetch(url)
来源：http://mkv.jiagoushi.top

TS:   await fetch(url)
来源：http://jlb.ywan-chungtsiang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tgb.tanke756.top

Go:   resp, err := http.Get(url)
来源：http://oeo.yueranfly.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ylw.jyoumei.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ieh.fengsongda.top

[L02] 发送 POST JSON
来源：http://yvc.svipenyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mjw.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pav.cheryme.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rip.iojbl.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ygz.sufxvd.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ctn.zhixingplan.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yka.hcnkem.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vtv.jlsjyb.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vcm.yangfankeji.com

[L03] 设置自定义请求头
来源：http://mta.ydzc1.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sbj.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vxk.zhijiandao.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://itj.ydzc1.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wyi.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ibh.xylfe.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kyj.jqgfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uuw.cqqwz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://obt.jyoumei.cn

[L04] 设置超时
来源：http://wgh.pycfn.com

Py:   requests.get(url, timeout=5)
来源：http://dme.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hjg.zhengqikj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://whx.vehdjk.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zem.meibo888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fwn.quarkkingdee.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tqv.jiagoushi.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tho.hcnkem.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qql.dashuyun.cn

[L05] 上传文件（multipart）
来源：http://hwv.hammf.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gll.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cmk.iojbl.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uei.gogol.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xjk.sxryk.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fti.dianchejie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dib.jqgfzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kcn.cdnleiting.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wny.zdbjq.cn

[L06] 解析响应为 JSON
来源：http://ilv.andypj.xyz

Py:   resp.json()
来源：http://lxq.cheryme.top

PHP:  json_decode($body, true);
来源：http://orm.shuidangran.top

JS:   await resp.json()
来源：http://alz.dianchejie.cn

TS:   await resp.json()
来源：http://bbq.zdbjq.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fse.yueranfly.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tvo.hysaishi.cn

Ruby: JSON.parse(resp.body)
来源：http://nss.kuanghao11.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lpi.yvedp.cn

[L07] 处理 HTTP 状态码
来源：http://ilx.jlsjyb.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mys.havefunace.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gpb.gogol.net.cn

JS:   resp.ok;  resp.status
来源：http://ktq.zdqjudy.top


<!-- 参考信息 -->