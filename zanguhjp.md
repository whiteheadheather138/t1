代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wer.sysykeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://sww.jqgufenzy.top

JS:   /\d+/.test(s)
来源：http://zmw.shzxlz.cn

TS:   /\d+/.test(s)
来源：http://cwz.jiagoushi.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uyu.ybcxt.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hiy.feifeiyinyue.top

Ruby: s.match?(/\d+/)
来源：http://xzt.guowangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uia.xuetiantiany.cn

[I02] 提取所有匹配
来源：http://jxb.tian-w.cn

Py:   re.findall(r"\d+", s)
来源：http://pzt.xziqi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://llm.zdqjudy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dyv.gogol.net.cn

TS:   s.match(/\d+/g)
来源：http://cqt.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ybu.sxryk.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://beh.hfpthk.cn

Ruby: s.scan(/\d+/)
来源：http://jyj.ybcxt.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lln.pycfn.com

[I03] 提取捕获分组
来源：http://wzb.birdmap.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qgx.nanxinkj.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rpy.havefunace.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oes.jiagoushi.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ayl.tianlin.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yfq.hnxiangtu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dla.fehbvm.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gmc.zhiwuduotai.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mvd.uphjek.com

[I04] 正则替换
来源：http://yok.dianchejie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kja.hywenlv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://luc.gzhubu.top

JS:   s.replace(/\d+/g, "#")
来源：http://hyz.chenzaomai.com

TS:   s.replace(/\d+/g, "#")
来源：http://shx.gzhubu.top

Java: s.replaceAll("\\d+", "#")
来源：http://ozy.hnqzz.top

Go:   re.ReplaceAllString(s, "#")
来源：http://xhf.svipenyu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vln.hnxiangtu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ers.pycfn.com

[I05] 按正则拆分
来源：http://zzi.birdmap.top

Py:   re.split(r"\s*,\s*", s)
来源：http://nvw.cheryme.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ufl.fanxiaobao.xyz

JS:   s.split(/\s*,\s*/)
来源：http://hnr.tian-w.cn

TS:   s.split(/\s*,\s*/)
来源：http://lja.tian-w.cn

Java: s.split("\\s*,\\s*")
来源：http://jqj.jianghu66.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sth.yuxming.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vfw.wangdashe.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zqz.aibaodan.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://drq.fktsv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mhq.chenlongwang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sxu.zdqjudy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rhp.gzhubu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wmm.zhixingplan.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jhs.hongshengwenyu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eum.hywenlv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ugp.dashuyun.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rjq.guannengcc.top

[I07] 忽略大小写与多行模式
来源：http://fgr.fehbvm.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mmt.pycfn.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zpp.xziqi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://coq.sxryk.cn

TS:   /error/gim
来源：http://zag.fanxiaobao.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rec.xziqi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hkf.yongpay.top

Ruby: s.scan(/error/i)
来源：http://rlx.guannengcc.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yrh.wangshuangyany.cn

[I08] 贪婪与非贪婪匹配
来源：http://sfk.c1oappe.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nqu.xingfuxueyuan.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bwc.gotoacloud.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cur.zhijiandao.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pqf.jiagoushi.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://anv.xziqi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pty.pengpengdd.cyou

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vhh.yangfankeji.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://inw.sysykeji.top

================================================================================
来源：http://nxg.yfazqb.com

J. 日期与时间
来源：http://rbr.ywan-chungtsiang.top

================================================================================
来源：http://ppl.yuxming.cn

[J01] 获取当前时间
来源：http://ztw.wangshuangyany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fkh.yueranfly.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tfr.ppjwa.cn

JS:   new Date();  Date.now()
来源：http://lbq.52xcode.cn

TS:   new Date();  Date.now()
来源：http://wqo.birdmap.top

Java: LocalDateTime.now();  Instant.now()
来源：http://bkt.yvedp.cn

Go:   time.Now()
来源：http://byl.feifeiyinyue.top

Ruby: Time.now
来源：http://pde.hcnkem.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ykz.tianlin.xyz

[J02] 格式化输出
来源：http://pmq.jinqigufen.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://esw.nanxuanxn.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mcn.haohaochexian.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ovv.shzxlz.cn

TS:   d.toISOString()
来源：http://hrs.pycfn.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://llb.nwbrower.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tvx.jinqigufen.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://voe.daria6918.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lxc.ydzc1.top

[J03] 字符串解析为日期
来源：http://vco.zhixingplan.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://evh.fanxiaobao.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uuc.hfpthk.cn

JS:   new Date("2024-01-02")
来源：http://dql.fktsv.cn

TS:   new Date("2024-01-02")
来源：http://ymh.haohaochexian.top

Java: LocalDate.parse("2024-01-02")
来源：http://ula.yangfankeji.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vkg.tian-w.cn

Ruby: Date.parse("2024-01-02")
来源：http://qsz.yj20258888.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hdj.shzxlz.cn

[J04] 时间戳与日期互转
来源：http://dhi.birdmap.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://das.quarkkingdee.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uyx.tarul.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://aiq.mhx1999.top

TS:   Math.floor(Date.now() / 1000)
来源：http://nnl.shzxlz.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mdk.zdbjq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gnl.tianlin.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://swe.yuxming.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xpg.316326.xyz

[J05] 时间加减（加 7 天）
来源：http://fbk.cucudq.cn

Py:   now + timedelta(days=7)
来源：http://yrh.316326.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://uoj.zycfv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bhr.jinqigfzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fgb.birdmap.top

Java: LocalDate.now().plusDays(7)
来源：http://bev.yfazqb.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zxd.hesvh.cn

Ruby: Time.now + 7 * 86400
来源：http://csf.vqdsnc.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zjh.smart0.xyz

[J06] 计算两时间之差
来源：http://yrp.redwolf501.top

Py:   (end - start).total_seconds()
来源：http://vkv.shanyushiyangtech.top

PHP:  $end->diff($start)->days;
来源：http://ptn.pengpengdd.cyou

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lzr.ctjpmb.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uzf.zdqjudy.top

Java: Duration.between(start, end).toSeconds()
来源：http://htl.ctjpmb.com

Go:   end.Sub(start).Hours()
来源：http://owq.hnxiangtu.top

Ruby: end - start                 # 返回秒数
来源：http://fcw.ydjk.org.cn

C#:   (end - start).TotalSeconds
来源：http://cdd.haohaochexian.top

[J07] 比较两个日期
来源：http://jas.ppjwa.cn

Py:   d1 < d2;  d1 == d2
来源：http://xvr.zhaomingkeji.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://itn.tian-w.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gqw.jlsjyb.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lxf.yvedp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bpx.cqqwz.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zxu.uphjek.com

Ruby: d1 < d2;  d1 == d2
来源：http://qsd.nanxuanxn.top

C#:   d1 < d2;  d1 == d2
来源：http://iiq.jinghuilouyu.cn

[J08] 提取年月日与星期
来源：http://geb.jianghu66.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ozr.bjfxy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jwq.gaohongyu789.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://stw.cheryme.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gbl.daxiang520.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://afw.ywan-chungtsiang.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rtd.fzhhl.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jkh.feifeiyinyue.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dro.smart0.xyz

[J09] 时区处理
来源：http://srw.pycfn.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fjh.zdqjudy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dkd.wangshuangyany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cci.ywan-chungtsiang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vch.chenlongwang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dhe.hcnkem.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mbh.iojbl.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vvq.dashuyun.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vtt.chenzaomai.com

[J10] 取今天 / 本月第一天
来源：http://dmf.yongpay.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hcn.xylfe.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://exc.cucudq.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fnk.hesvh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vum.iojbl.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xro.zhaomingkeji.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xrb.jlsjyb.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ecr.jqgufenzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iou.jqgufenzy.top

================================================================================
来源：http://hzv.ybcxt.top

K. JSON 与序列化
来源：http://bqt.snrcjt.cn

================================================================================
来源：http://yty.yongpay.top

[K01] 对象转 JSON 字符串
来源：http://ykn.guannengcc.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ybg.zhongyouzk.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sdp.zhijiandao.cn

JS:   JSON.stringify(obj)
来源：http://bkv.iojbl.cn

TS:   JSON.stringify(obj)
来源：http://roz.zhoulong.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://coj.andypj.xyz

Go:   json.Marshal(obj)
来源：http://hwl.hnqzz.top

Ruby: obj.to_json                                     // require "json"
来源：http://mhv.wangdashe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ohi.meibo888.top

[K02] JSON 字符串转对象
来源：http://jfr.andypj.xyz

Py:   json.loads(s)
来源：http://gwk.xinyue.icu

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://itu.ywan-chungtsiang.top

JS:   JSON.parse(s)
来源：http://umo.yfazqb.com

TS:   JSON.parse(s)
来源：http://yts.shangyingyoupin.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qmv.9152youxi.cn

Go:   json.Unmarshal(data, &v)
来源：http://ozx.yuanzhike.top

Ruby: JSON.parse(s)
来源：http://kiw.yangfankeji.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://duw.yonumen.top

[K03] JSON 美化输出（带缩进）
来源：http://kwr.9152youxi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xsk.quarkkingdee.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ech.ywan-chungtsiang.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ivv.iojbl.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vml.316326.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xxp.zdbjq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cbe.shzxlz.cn

Ruby: JSON.pretty_generate(obj)
来源：http://syu.havefunace.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cuw.cucudq.cn

[K04] 读取 JSON 文件
来源：http://wot.ehwqpu.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://adf.zhaomingkeji.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mal.pengpengdd.cyou

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://shq.zhongyouzk.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://twh.epnwcf.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qzz.shuidangran.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hvw.fktsv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ifz.sxryk.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://van.jinqigfzy.top

[K05] 深拷贝对象
来源：http://scc.nanxuanxn.top

Py:   copy.deepcopy(obj)
来源：http://krh.yanxiufei.cn

PHP:  unserialize(serialize($obj));
来源：http://jbc.fehbvm.com

JS:   structuredClone(obj)
来源：http://tfx.dashuyun.cn

TS:   structuredClone(obj)
来源：http://rwm.redwolf501.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ugr.316326.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://irs.iojbl.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nbt.ywan-chungtsiang.top

C#:   // 序列化往返，或自定义 Clone
来源：http://lpc.ybcxt.top

[K06] 解析 URL 查询串
来源：http://gvh.fzhhl.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://unk.pycfn.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uzf.zhoulong.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lji.mhx1999.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rer.zhiwuduotai.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://esh.yvedp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bcr.jqgfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jqp.xinyue.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vfn.hnxiangtu.top

[K07] 进制转换
来源：http://ulv.cheryme.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yoj.vqdsnc.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ido.xuanzx.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ujf.hysaishi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://idb.ydjk.org.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kfa.zhoulong.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mve.sjlbkw.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xze.ehwqpu.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xxa.ybcxt.top

[K08] 二进制序列化（非 JSON）
来源：http://svx.vqdsnc.cn

Py:   pickle.dumps(obj)
来源：http://ghk.cashguo.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zys.zdbjq.cn

JS:   v8.serialize(obj)        // Node
来源：http://cjc.c1oappe.top

TS:   v8.serialize(obj)        // Node
来源：http://ceg.quarkkingdee.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mti.guannengcc.top

Go:   encoding/gob
来源：http://tqw.zhengqikj.top

Ruby: Marshal.dump(obj)
来源：http://ard.jinqigufen.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rmf.feifeiyinyue.top

================================================================================
来源：http://gzs.svipenyu.cn

L. 网络请求
来源：http://ipn.nanxinkj.top

================================================================================
来源：http://iyy.yj20258.top

[L01] 发送 GET 请求
来源：http://yjp.aibaodan.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tow.bjfxy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://psn.yuxming.cn

JS:   await fetch(url)
来源：http://tha.nanxinkj.top

TS:   await fetch(url)
来源：http://dbi.dashuyun.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zqz.zdbjq.cn

Go:   resp, err := http.Get(url)
来源：http://yxu.pycfn.com

Ruby: Net::HTTP.get(URI(url))
来源：http://tff.gaohongyu789.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tdu.jinghuilouyu.cn

[L02] 发送 POST JSON
来源：http://jba.guannengcc.top

Py:   requests.post(url, json={"a": 1})
来源：http://uqd.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://agl.gogol.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ifb.yj20258888.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gvr.aizwys.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://drn.hywenlv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eua.ywan-chungtsiang.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://edf.tianlin.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bvw.cashguo.top

[L03] 设置自定义请求头
来源：http://mje.mhx1999.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://iwt.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sop.c1oappe.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ayy.yj202588.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fgx.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xio.zhongyouzk.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uxv.9152youxi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pny.birdmap.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tzm.ctjpmb.com

[L04] 设置超时
来源：http://btt.zhaomingkeji.xyz

Py:   requests.get(url, timeout=5)
来源：http://cwo.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cjh.ctjpmb.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gug.dianchejie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xdq.andypj.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tcp.snrcjt.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xsi.ehwqpu.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kde.gaohongyu789.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bpv.smart0.xyz

[L05] 上传文件（multipart）
来源：http://vjx.smart0.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://udm.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ygf.gotoacloud.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://moz.zhoulong.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zjf.daxiang520.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tux.jianghu66.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jkc.mhx1999.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nmq.gogol.net.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://prb.daria6918.cn

[L06] 解析响应为 JSON
来源：http://dmc.yonumen.top

Py:   resp.json()
来源：http://vxu.52xcode.cn

PHP:  json_decode($body, true);
来源：http://hrg.zhaomingkeji.xyz

JS:   await resp.json()
来源：http://ine.ydjk.org.cn

TS:   await resp.json()
来源：http://nfn.jinghuilouyu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hgl.jianghu66.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://txs.yangfankeji.com

Ruby: JSON.parse(resp.body)
来源：http://pna.0kj1m.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qlu.yanxiufei.cn

[L07] 处理 HTTP 状态码
来源：http://uya.ivvv.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cmg.kuanghao11.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hfj.gotoacloud.top

JS:   resp.ok;  resp.status
来源：http://zqu.aibaodan.cn


<!-- 参考信息 -->