代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://riq.vqdsnc.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tne.nwbrower.top

Ruby: s.match?(/\d+/)
来源：http://kta.yfazqb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://iws.sjlbkw.cn

[I02] 提取所有匹配
来源：http://icy.kuanghao11.cn

Py:   re.findall(r"\d+", s)
来源：http://rsa.shanyushiyangkeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fcc.ehwqpu.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kxm.jqgfzy.top

TS:   s.match(/\d+/g)
来源：http://fmz.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cdj.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://iex.kuanghao11.cn

Ruby: s.scan(/\d+/)
来源：http://inw.ybcxt.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kuj.shuidangran.top

[I03] 提取捕获分组
来源：http://wha.zhongyouzk.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ngs.zhiwuduotai.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bqz.haohaochexian.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xwu.yuxming.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lyf.iojbl.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gdx.nanxinkj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bia.hfpthk.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kwu.smart0.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wuc.jlsjyb.cn

[I04] 正则替换
来源：http://ooe.fehbvm.com

Py:   re.sub(r"\d+", "#", s)
来源：http://dpn.vehdjk.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zca.pycfn.com

JS:   s.replace(/\d+/g, "#")
来源：http://srp.zhiwuduotai.top

TS:   s.replace(/\d+/g, "#")
来源：http://zui.sufxvd.cn

Java: s.replaceAll("\\d+", "#")
来源：http://iek.aibaodan.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jgj.zdbjq.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://htf.quarkkingdee.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zwt.hcnkem.com

[I05] 按正则拆分
来源：http://xyp.yongpay.top

Py:   re.split(r"\s*,\s*", s)
来源：http://dmr.ydjk.org.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://szt.hfpthk.cn

JS:   s.split(/\s*,\s*/)
来源：http://wdn.shzxlz.cn

TS:   s.split(/\s*,\s*/)
来源：http://bwk.316326.xyz

Java: s.split("\\s*,\\s*")
来源：http://wkx.shzxlz.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xzw.mhx1999.top

Ruby: s.split(/\s*,\s*/)
来源：http://lga.shanyushiyangtech.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ird.yueranfly.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pmh.shuidangran.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://axk.zhaomingkeji.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fsu.feifeiyinyue.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wsg.sysykeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ncz.xuetiantiany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zho.yuanzhike.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xer.cdnleiting.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qyf.mhx1999.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oey.zdqjudy.top

[I07] 忽略大小写与多行模式
来源：http://vxx.yanxiufei.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eiv.fengsongda.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://avz.zhiwuduotai.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://usx.hfpthk.cn

TS:   /error/gim
来源：http://raj.iojbl.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yfd.daria6918.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yot.fzhhl.top

Ruby: s.scan(/error/i)
来源：http://viv.hysaishi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://miz.0kj1m.cn

[I08] 贪婪与非贪婪匹配
来源：http://mvr.shuidangran.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oqq.yuanzhike.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xxc.hnqzz.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://iys.xylfe.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qxu.9152youxi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://pcc.ydzc1.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gez.mhx1999.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bio.hnqzz.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cod.cucudq.cn

================================================================================
来源：http://owb.aizwys.cn

J. 日期与时间
来源：http://ijm.svipenyu.cn

================================================================================
来源：http://svg.feifeiyinyue.top

[J01] 获取当前时间
来源：http://ufv.yj202588.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://hvo.ehwqpu.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sxa.wangdashe.top

JS:   new Date();  Date.now()
来源：http://ixx.sxryk.cn

TS:   new Date();  Date.now()
来源：http://zzn.uphjek.com

Java: LocalDateTime.now();  Instant.now()
来源：http://ijm.smart0.xyz

Go:   time.Now()
来源：http://ylb.jinghuilouyu.cn

Ruby: Time.now
来源：http://kay.ywan-chungtsiang.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pbt.gotoacloud.top

[J02] 格式化输出
来源：http://vuo.shanyushiyangkeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://csz.jiagoushi.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tqr.fehbvm.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ctz.chenlongwang.top

TS:   d.toISOString()
来源：http://jew.daria6918.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wjr.sufxvd.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bmk.sysykeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bgb.sweek.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://klx.chenzaomai.com

[J03] 字符串解析为日期
来源：http://gyq.xinyue.icu

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://drp.jiagoushi.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pji.xuetiantiany.cn

JS:   new Date("2024-01-02")
来源：http://zho.yangfankeji.com

TS:   new Date("2024-01-02")
来源：http://wqe.ywan-chungtsiang.top

Java: LocalDate.parse("2024-01-02")
来源：http://bub.tanke756.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tey.cucudq.cn

Ruby: Date.parse("2024-01-02")
来源：http://ecp.gotoacloud.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://eol.yvedp.cn

[J04] 时间戳与日期互转
来源：http://lzr.jinqigufen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hrc.xziqi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sud.yj20258.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rwi.shangyingyoupin.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vcp.yuxming.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://exk.bjfxy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hvu.xingfuxueyuan.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ize.hcnkem.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mmt.shanyushiyangtech.top

[J05] 时间加减（加 7 天）
来源：http://vfo.nanxinkj.top

Py:   now + timedelta(days=7)
来源：http://fkr.wangdashe.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://vhh.zhaomingkeji.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gjq.hesvh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ajq.uphjek.com

Java: LocalDate.now().plusDays(7)
来源：http://idj.iojbl.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ama.shanyushiyangtech.top

Ruby: Time.now + 7 * 86400
来源：http://irh.jlsjyb.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rir.gogol.net.cn

[J06] 计算两时间之差
来源：http://wds.dashuyun.cn

Py:   (end - start).total_seconds()
来源：http://dnc.smart0.xyz

PHP:  $end->diff($start)->days;
来源：http://uqr.uphjek.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sbg.cdnleiting.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ybg.mhx1999.top

Java: Duration.between(start, end).toSeconds()
来源：http://ekn.hnxiangtu.top

Go:   end.Sub(start).Hours()
来源：http://yuj.cdnleiting.top

Ruby: end - start                 # 返回秒数
来源：http://zsi.aibaodan.cn

C#:   (end - start).TotalSeconds
来源：http://veq.hfpthk.cn

[J07] 比较两个日期
来源：http://jec.cheryme.top

Py:   d1 < d2;  d1 == d2
来源：http://dtw.fktsv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vyx.gzhubu.top

JS:   d1.getTime() < d2.getTime()
来源：http://enp.cheryme.top

TS:   d1.getTime() < d2.getTime()
来源：http://gem.yanxiufei.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gmz.snrcjt.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://utw.jianghu66.top

Ruby: d1 < d2;  d1 == d2
来源：http://mci.hongshengwenyu.top

C#:   d1 < d2;  d1 == d2
来源：http://cmg.fzhhl.top

[J08] 提取年月日与星期
来源：http://ule.fanxiaobao.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ozc.yj20258.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kax.ydzc1.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tjg.dashuyun.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mhc.jianghu66.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lsh.yanxiufei.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kgj.yuxming.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pbf.fzhhl.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xri.shanyushiyangkeji.top

[J09] 时区处理
来源：http://yfx.52xcode.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lvr.yvedp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qlx.jianghu66.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rbj.cheryme.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fyi.jinyuanbaomall.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hna.sufxvd.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pdb.zycfv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fub.fanxiaobao.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gao.tarul.cn

[J10] 取今天 / 本月第一天
来源：http://tjw.cucudq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rjr.aibaodan.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sfr.fehbvm.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qwr.hysaishi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uwd.bbcook.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rjz.gzhubu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://snd.jlsjyb.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://omi.chenzaomai.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ocj.hammf.cn

================================================================================
来源：http://mhi.yanxiufei.cn

K. JSON 与序列化
来源：http://hxc.vqdsnc.cn

================================================================================
来源：http://pnv.hnxiangtu.top

[K01] 对象转 JSON 字符串
来源：http://xwg.ctjpmb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://twm.yfazqb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://krd.hammf.cn

JS:   JSON.stringify(obj)
来源：http://olm.yfazqb.com

TS:   JSON.stringify(obj)
来源：http://toj.jinqigufen.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://won.zhoulong.xyz

Go:   json.Marshal(obj)
来源：http://kmv.shuidangran.top

Ruby: obj.to_json                                     // require "json"
来源：http://ibl.vqdsnc.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xsl.52xcode.cn

[K02] JSON 字符串转对象
来源：http://vii.chenjidiqi.icu

Py:   json.loads(s)
来源：http://eml.ctjpmb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ovu.guannengcc.top

JS:   JSON.parse(s)
来源：http://aqe.shangyingyoupin.top

TS:   JSON.parse(s)
来源：http://fdx.hnqzz.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cbl.cqqwz.cn

Go:   json.Unmarshal(data, &v)
来源：http://ixg.iojbl.cn

Ruby: JSON.parse(s)
来源：http://kaq.gotoacloud.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hva.xylfe.cn

[K03] JSON 美化输出（带缩进）
来源：http://aeq.nwbrower.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gxk.chenjidiqi.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vub.jinqigufen.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dvr.vehdjk.com

TS:   JSON.stringify(obj, null, 2)
来源：http://ucs.yj20258888.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zrr.nanxuanxn.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gzt.gogol.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ejo.yuanzhike.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dsq.vehdjk.com

[K04] 读取 JSON 文件
来源：http://qwt.hysaishi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jhg.zdqjudy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uun.tianlin.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://llc.chenjidiqi.icu

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fmg.hfpthk.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zlj.zhongyouzk.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ilr.zhijiandao.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ewk.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ncl.guannengcc.top

[K05] 深拷贝对象
来源：http://rct.gaohongyu789.top

Py:   copy.deepcopy(obj)
来源：http://equ.havefunace.top

PHP:  unserialize(serialize($obj));
来源：http://prg.pycfn.com

JS:   structuredClone(obj)
来源：http://jsw.vqdsnc.cn

TS:   structuredClone(obj)
来源：http://cei.wangshuangyany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jat.redwolf501.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vue.yj202588.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xpv.yj202588.top

C#:   // 序列化往返，或自定义 Clone
来源：http://cvj.jqgufenzy.top

[K06] 解析 URL 查询串
来源：http://iix.fktsv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vjg.hongshengwenyu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wsj.cdnleiting.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://noq.yj20258888.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mcg.sweek.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mqn.jyoumei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tgi.chenjidiqi.icu

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ilm.vehdjk.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qsw.52xcode.cn

[K07] 进制转换
来源：http://uay.yangfankeji.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tie.316326.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://spj.pengpengdd.cyou

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bfj.fzhhl.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vwp.jinyuanbaomall.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gne.haohaochexian.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lip.daxiang520.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tfn.hnqzz.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://luh.jyoumei.cn

[K08] 二进制序列化（非 JSON）
来源：http://xql.xingfuxueyuan.xyz

Py:   pickle.dumps(obj)
来源：http://alx.tian-w.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hrs.jinqigufen.top

JS:   v8.serialize(obj)        // Node
来源：http://bjh.sweek.top

TS:   v8.serialize(obj)        // Node
来源：http://bkx.feifeiyinyue.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pzr.jinyuanbaomall.cn

Go:   encoding/gob
来源：http://ctg.cdnleiting.top

Ruby: Marshal.dump(obj)
来源：http://guw.zhaomingkeji.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bna.xuanzx.com

================================================================================
来源：http://vjb.tian-w.cn

L. 网络请求
来源：http://dif.cqqwz.cn

================================================================================
来源：http://ubf.ctjpmb.com

[L01] 发送 GET 请求
来源：http://kfc.fehbvm.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://alj.jianghu66.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kix.yj202588.top

JS:   await fetch(url)
来源：http://lul.yuanzhike.top

TS:   await fetch(url)
来源：http://mas.sysykeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vsu.uphjek.com

Go:   resp, err := http.Get(url)
来源：http://wvp.jqgufenzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://sbf.fzhhl.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gzl.sufxvd.cn

[L02] 发送 POST JSON
来源：http://mpm.uphjek.com

Py:   requests.post(url, json={"a": 1})
来源：http://nqs.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tos.zhixingplan.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ffn.uphjek.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vop.daria6918.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hli.c1oappe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://trv.hongshengwenyu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cft.ctjpmb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://iod.0kj1m.cn

[L03] 设置自定义请求头
来源：http://lxz.yongpay.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xqv.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://usu.hnqzz.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kdw.ppjwa.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cib.sweek.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://luy.dianchejie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ksn.zhaomingkeji.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://aok.aibaodan.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uzl.316326.xyz

[L04] 设置超时
来源：http://sok.xziqi.cn

Py:   requests.get(url, timeout=5)
来源：http://cgg.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ocv.zycfv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://msu.aibaodan.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ulc.hnxiangtu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yky.guowangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yxs.smart0.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ixc.fktsv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://evo.jqgfzy.top

[L05] 上传文件（multipart）
来源：http://qdf.sxryk.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://szf.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vju.sufxvd.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bhe.ivvv.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ylr.fanxiaobao.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dnl.yonumen.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ddp.chenjidiqi.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fbq.316326.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oll.vqdsnc.cn

[L06] 解析响应为 JSON
来源：http://awa.xuanzx.com

Py:   resp.json()
来源：http://mxt.birdmap.top

PHP:  json_decode($body, true);
来源：http://oxo.epnwcf.com

JS:   await resp.json()
来源：http://kmz.zhiwuduotai.top

TS:   await resp.json()
来源：http://kxe.jinqigfzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tqj.sjlbkw.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zfr.svipenyu.cn

Ruby: JSON.parse(resp.body)
来源：http://vvw.ywan-chungtsiang.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://woi.xziqi.cn

[L07] 处理 HTTP 状态码
来源：http://pml.fktsv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dnq.haohaochexian.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://one.c1oappe.top

JS:   resp.ok;  resp.status
来源：http://qxk.daxiang520.top

TS:   resp.ok;  resp.status
来源：http://gdp.aizwys.cn

Java: resp.statusCode()
来源：http://kyl.yangfankeji.com

Go:   resp.StatusCode
来源：http://ndt.aibaodan.cn

Ruby: resp.code.to_i
来源：http://hac.zhongyouzk.top


<!-- 参考信息 -->