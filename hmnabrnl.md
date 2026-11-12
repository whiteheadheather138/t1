代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://efg.zdqjudy.top

PHP:  preg_match('/\d+/', $s);
来源：http://krt.52xcode.cn

JS:   /\d+/.test(s)
来源：http://oxv.shuidangran.top

TS:   /\d+/.test(s)
来源：http://xpr.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mim.redwolf501.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xkj.aibaodan.cn

Ruby: s.match?(/\d+/)
来源：http://ujk.jyoumei.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://eag.hcnkem.com

[I02] 提取所有匹配
来源：http://anu.zycfv.cn

Py:   re.findall(r"\d+", s)
来源：http://kpe.hysaishi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vbr.xuanzx.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zcf.daxiang520.top

TS:   s.match(/\d+/g)
来源：http://cnc.c1oappe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wnb.yvedp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pdo.sjlbkw.cn

Ruby: s.scan(/\d+/)
来源：http://poj.jyoumei.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rsn.yuxming.cn

[I03] 提取捕获分组
来源：http://yzg.dashuyun.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yua.quarkkingdee.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://knf.jlsjyb.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wfm.0kj1m.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://knc.ywan-chungtsiang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hab.9152youxi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ezh.ybcxt.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gdz.ywan-chungtsiang.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zke.nanxinkj.top

[I04] 正则替换
来源：http://ens.sjlbkw.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://syb.hfpthk.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xwu.zhongyouzk.top

JS:   s.replace(/\d+/g, "#")
来源：http://mla.sjlbkw.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mzz.vehdjk.com

Java: s.replaceAll("\\d+", "#")
来源：http://xbb.xingfuxueyuan.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://hup.hnxiangtu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://sqv.hnxiangtu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nmx.wangshuangyany.cn

[I05] 按正则拆分
来源：http://hhv.meibo888.top

Py:   re.split(r"\s*,\s*", s)
来源：http://pae.yj20258.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ffh.zdqjudy.top

JS:   s.split(/\s*,\s*/)
来源：http://bai.cqqwz.cn

TS:   s.split(/\s*,\s*/)
来源：http://pgd.havefunace.top

Java: s.split("\\s*,\\s*")
来源：http://zph.sysykeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mjw.birdmap.top

Ruby: s.split(/\s*,\s*/)
来源：http://bmn.vqdsnc.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yhh.mhx1999.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://aio.hnqzz.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://owb.sweek.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cfe.yongpay.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tjt.mhx1999.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jvy.yfazqb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xlb.fzhhl.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jcy.shangyingyoupin.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qtu.pycfn.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://glj.316326.xyz

[I07] 忽略大小写与多行模式
来源：http://zgd.jlsjyb.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jqe.xinyue.icu

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://snk.cqqwz.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iye.kuanghao11.cn

TS:   /error/gim
来源：http://svo.zdbjq.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://aii.zhixingplan.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hcs.hongshengwenyu.top

Ruby: s.scan(/error/i)
来源：http://noe.ywan-chungtsiang.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://eah.zdbjq.cn

[I08] 贪婪与非贪婪匹配
来源：http://ddu.kuanghao11.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://msw.epnwcf.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rac.52xcode.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gjp.fktsv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rij.ctjpmb.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://ucu.xinyue.icu

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://suh.zhaomingkeji.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://icv.guannengcc.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://arr.zycfv.cn

================================================================================
来源：http://amx.xinyue.icu

J. 日期与时间
来源：http://udh.yj20258.top

================================================================================
来源：http://dss.chenlongwang.top

[J01] 获取当前时间
来源：http://svl.ywan-chungtsiang.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://yyx.vehdjk.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rxq.yanxiufei.cn

JS:   new Date();  Date.now()
来源：http://acs.yueranfly.top

TS:   new Date();  Date.now()
来源：http://pah.andypj.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://nyh.pengpengdd.cyou

Go:   time.Now()
来源：http://rxx.zycfv.cn

Ruby: Time.now
来源：http://lzo.andypj.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oxl.hysaishi.cn

[J02] 格式化输出
来源：http://tzb.zhiwuduotai.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vlv.fanxiaobao.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://meh.jqgufenzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://svb.tanke756.top

TS:   d.toISOString()
来源：http://jmt.52xcode.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bsu.ivvv.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gti.shzxlz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fkd.shzxlz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://igp.xziqi.cn

[J03] 字符串解析为日期
来源：http://xyq.andypj.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mes.hesvh.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jnt.sjlbkw.cn

JS:   new Date("2024-01-02")
来源：http://vka.jiagoushi.top

TS:   new Date("2024-01-02")
来源：http://ddb.ivvv.top

Java: LocalDate.parse("2024-01-02")
来源：http://ace.ivvv.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rlx.shangyingyoupin.top

Ruby: Date.parse("2024-01-02")
来源：http://mck.pycfn.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gkd.yj20258888.top

[J04] 时间戳与日期互转
来源：http://uhr.ivvv.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ssn.hongshengwenyu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qug.fehbvm.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://otr.nwbrower.top

TS:   Math.floor(Date.now() / 1000)
来源：http://dpn.ybcxt.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kck.cucudq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lgh.xuanzx.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lwi.svipenyu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pep.dashuyun.cn

[J05] 时间加减（加 7 天）
来源：http://plr.fktsv.cn

Py:   now + timedelta(days=7)
来源：http://wut.uphjek.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://chr.cqqwz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ccj.pycfn.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fus.cheryme.top

Java: LocalDate.now().plusDays(7)
来源：http://ruz.yj20258888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kwh.shanyushiyangtech.top

Ruby: Time.now + 7 * 86400
来源：http://dfe.shanyushiyangkeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://vtt.cucudq.cn

[J06] 计算两时间之差
来源：http://zid.ivvv.top

Py:   (end - start).total_seconds()
来源：http://cai.c1oappe.top

PHP:  $end->diff($start)->days;
来源：http://ive.nwbrower.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tgs.chenzaomai.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ngo.havefunace.top

Java: Duration.between(start, end).toSeconds()
来源：http://flr.yangfankeji.com

Go:   end.Sub(start).Hours()
来源：http://dyc.kuanghao11.cn

Ruby: end - start                 # 返回秒数
来源：http://hyg.0kj1m.cn

C#:   (end - start).TotalSeconds
来源：http://nyu.jianghu66.top

[J07] 比较两个日期
来源：http://tgn.aibaodan.cn

Py:   d1 < d2;  d1 == d2
来源：http://ust.xingfuxueyuan.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://msg.ywan-chungtsiang.top

JS:   d1.getTime() < d2.getTime()
来源：http://upe.ehwqpu.com

TS:   d1.getTime() < d2.getTime()
来源：http://egf.jinghuilouyu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xgf.mhx1999.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://drc.jinyuanbaomall.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rgq.yongpay.top

C#:   d1 < d2;  d1 == d2
来源：http://bmv.yj20258.top

[J08] 提取年月日与星期
来源：http://bzz.fehbvm.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wfw.chenlongwang.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fyn.jlsjyb.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ppz.jlsjyb.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://anh.uphjek.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dqu.jiagoushi.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lsj.cqqwz.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fue.zycfv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://slv.pengpengdd.cyou

[J09] 时区处理
来源：http://wnq.cheryme.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fqb.andypj.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cqj.shuidangran.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cxt.fktsv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hoe.jyoumei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pzg.haohaochexian.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mnm.ydjk.org.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xix.shuidangran.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tvu.fanxiaobao.xyz

[J10] 取今天 / 本月第一天
来源：http://gwa.jlsjyb.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wux.gotoacloud.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://stq.birdmap.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zgo.ehwqpu.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ryi.svipenyu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mnq.vehdjk.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vso.wangshuangyany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ihw.zhengqikj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gzl.hammf.cn

================================================================================
来源：http://jmd.jqgfzy.top

K. JSON 与序列化
来源：http://wwe.cqqwz.cn

================================================================================
来源：http://skd.iojbl.cn

[K01] 对象转 JSON 字符串
来源：http://tgq.sysykeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ajj.vqdsnc.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rkj.nanxuanxn.top

JS:   JSON.stringify(obj)
来源：http://ofv.yueranfly.top

TS:   JSON.stringify(obj)
来源：http://ify.shzxlz.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ybq.yueranfly.top

Go:   json.Marshal(obj)
来源：http://nzs.hcnkem.com

Ruby: obj.to_json                                     // require "json"
来源：http://ige.guowangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://aon.gaohongyu789.top

[K02] JSON 字符串转对象
来源：http://pez.quarkkingdee.top

Py:   json.loads(s)
来源：http://lxd.zhoulong.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tzo.daria6918.cn

JS:   JSON.parse(s)
来源：http://gmb.cqqwz.cn

TS:   JSON.parse(s)
来源：http://vaj.hfpthk.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mdt.jinqigfzy.top

Go:   json.Unmarshal(data, &v)
来源：http://lct.zhoulong.xyz

Ruby: JSON.parse(s)
来源：http://piu.dashuyun.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://olt.nwbrower.top

[K03] JSON 美化输出（带缩进）
来源：http://tjr.xylfe.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hyn.pycfn.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pai.tian-w.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fso.wangshuangyany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sta.yonumen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ajw.xuanzx.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://grr.zdbjq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xmd.yuanzhike.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gpr.ivvv.top

[K04] 读取 JSON 文件
来源：http://vin.fktsv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://otq.ywan-chungtsiang.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ita.nanxuanxn.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mwo.fanxiaobao.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fhd.cheryme.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vxc.snrcjt.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sto.wangdashe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jug.daxiang520.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mvp.fzhhl.top

[K05] 深拷贝对象
来源：http://zli.hnqzz.top

Py:   copy.deepcopy(obj)
来源：http://qrq.quarkkingdee.top

PHP:  unserialize(serialize($obj));
来源：http://cfl.mhx1999.top

JS:   structuredClone(obj)
来源：http://fab.gotoacloud.top

TS:   structuredClone(obj)
来源：http://tgu.zhiwuduotai.top

Java: // 手写拷贝构造，或序列化往返
来源：http://lzm.zhiwuduotai.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kfb.jqgufenzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zmd.hcnkem.com

C#:   // 序列化往返，或自定义 Clone
来源：http://bpc.hcnkem.com

[K06] 解析 URL 查询串
来源：http://oqz.jiagoushi.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xif.jqgufenzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://iok.nanxuanxn.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hce.epnwcf.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gyw.ppjwa.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ruj.ctjpmb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://mdu.yuxming.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jpn.ehwqpu.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bah.hongshengwenyu.top

[K07] 进制转换
来源：http://krr.ppjwa.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://udq.daria6918.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://egy.bjfxy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://arx.bjfxy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mpc.tian-w.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://upg.smart0.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jst.nanxuanxn.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fmj.redwolf501.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bko.shanyushiyangkeji.top

[K08] 二进制序列化（非 JSON）
来源：http://hgx.zhiwuduotai.top

Py:   pickle.dumps(obj)
来源：http://tgp.ctjpmb.com

PHP:  serialize($obj);  unserialize($s);
来源：http://nlx.andypj.xyz

JS:   v8.serialize(obj)        // Node
来源：http://ktp.nanxinkj.top

TS:   v8.serialize(obj)        // Node
来源：http://vjx.aizwys.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kfl.jinghuilouyu.cn

Go:   encoding/gob
来源：http://jtq.chenzaomai.com

Ruby: Marshal.dump(obj)
来源：http://won.jinqigfzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xvw.bjfxy.top

================================================================================
来源：http://psy.ydzc1.top

L. 网络请求
来源：http://pnm.jinghuilouyu.cn

================================================================================
来源：http://jdh.zdbjq.cn

[L01] 发送 GET 请求
来源：http://pbr.kuanghao11.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bhc.ctjpmb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zma.vqdsnc.cn

JS:   await fetch(url)
来源：http://doi.fehbvm.com

TS:   await fetch(url)
来源：http://jyx.jyoumei.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sfi.aibaodan.cn

Go:   resp, err := http.Get(url)
来源：http://ydm.shuidangran.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kzx.hnxiangtu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bkz.vehdjk.com

[L02] 发送 POST JSON
来源：http://ikt.shanyushiyangkeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://tfn.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hnw.hammf.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cei.daxiang520.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kni.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qib.zycfv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rva.ivvv.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jcm.ivvv.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wnn.yuanzhike.top

[L03] 设置自定义请求头
来源：http://myq.vehdjk.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hhw.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jyf.chenlongwang.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fhy.xuetiantiany.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ngc.yuanzhike.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rts.chenlongwang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ooc.nanxuanxn.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fma.52xcode.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vje.uphjek.com

[L04] 设置超时
来源：http://iol.hywenlv.cn

Py:   requests.get(url, timeout=5)
来源：http://wfw.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://guv.yanxiufei.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cko.zhoulong.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vsw.dianchejie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gug.0kj1m.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gwc.ppjwa.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jtg.hesvh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wyo.zhijiandao.cn

[L05] 上传文件（multipart）
来源：http://lvi.yanxiufei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nhd.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vwl.zhengqikj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gkz.chenjidiqi.icu

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://elw.xuanzx.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://adt.yuanzhike.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uyj.vehdjk.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bsh.yangfankeji.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qez.jinyuanbaomall.cn

[L06] 解析响应为 JSON
来源：http://dzb.yj20258.top

Py:   resp.json()
来源：http://oaf.vqdsnc.cn

PHP:  json_decode($body, true);
来源：http://ioa.iojbl.cn

JS:   await resp.json()
来源：http://ltb.chenzaomai.com

TS:   await resp.json()
来源：http://qui.cucudq.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dcq.jiagoushi.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ilt.9152youxi.cn

Ruby: JSON.parse(resp.body)
来源：http://juz.sjlbkw.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://otg.dianchejie.cn

[L07] 处理 HTTP 状态码
来源：http://tlg.xuetiantiany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kqz.hfpthk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fta.tarul.cn

JS:   resp.ok;  resp.status
来源：http://jon.gotoacloud.top


<!-- 参考信息 -->