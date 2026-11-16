代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xlw.316326.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://cdt.aibaodan.cn

JS:   /\d+/.test(s)
来源：http://mom.hnqzz.top

TS:   /\d+/.test(s)
来源：http://ydl.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nyw.guannengcc.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sou.wangshuangyany.cn

Ruby: s.match?(/\d+/)
来源：http://tqh.wangdashe.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fen.wangdashe.top

[I02] 提取所有匹配
来源：http://zjw.c1oappe.top

Py:   re.findall(r"\d+", s)
来源：http://bbp.ydzc1.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jaz.yfazqb.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ewd.jinqigfzy.top

TS:   s.match(/\d+/g)
来源：http://eqr.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qrv.c1oappe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hrk.smart0.xyz

Ruby: s.scan(/\d+/)
来源：http://brj.fengsongda.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lww.fktsv.cn

[I03] 提取捕获分组
来源：http://bwv.xylfe.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xmf.zhixingplan.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://shp.shanyushiyangkeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qaz.xinyue.icu

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gyk.fktsv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cxi.yueranfly.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://imb.yanxiufei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pdd.zdqjudy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://opo.nwbrower.top

[I04] 正则替换
来源：http://cmt.fanxiaobao.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://fqn.mhx1999.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cax.sjlbkw.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ijo.ppjwa.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yny.zhijiandao.cn

Java: s.replaceAll("\\d+", "#")
来源：http://une.pengpengdd.cyou

Go:   re.ReplaceAllString(s, "#")
来源：http://ltb.sxryk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fzp.meibo888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yrf.yfazqb.com

[I05] 按正则拆分
来源：http://uen.yj202588.top

Py:   re.split(r"\s*,\s*", s)
来源：http://htv.xingfuxueyuan.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://upb.cheryme.top

JS:   s.split(/\s*,\s*/)
来源：http://xgn.jinyuanbaomall.cn

TS:   s.split(/\s*,\s*/)
来源：http://cuq.gotoacloud.top

Java: s.split("\\s*,\\s*")
来源：http://pkh.jqgufenzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zge.wangdashe.top

Ruby: s.split(/\s*,\s*/)
来源：http://fny.shanyushiyangkeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kpl.fanxiaobao.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nyr.jlsjyb.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nch.yj202588.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dmh.zhoulong.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ujp.hnxiangtu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rqg.yongpay.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jcp.yj20258.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://phh.chenzaomai.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dci.nanxinkj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://axx.daxiang520.top

[I07] 忽略大小写与多行模式
来源：http://vkm.9152youxi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ulv.jqgfzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://shg.snrcjt.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://agx.hysaishi.cn

TS:   /error/gim
来源：http://joe.wangshuangyany.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mar.jiagoushi.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fwg.gzhubu.top

Ruby: s.scan(/error/i)
来源：http://nlp.jqgfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fdq.zhengqikj.top

[I08] 贪婪与非贪婪匹配
来源：http://klb.hfpthk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oto.yj20258.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ljb.ydzc1.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rvr.pycfn.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jyb.snrcjt.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ebs.nanxinkj.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qrq.hnxiangtu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mhq.chenzaomai.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hlv.havefunace.top

================================================================================
来源：http://ear.c1oappe.top

J. 日期与时间
来源：http://wrz.kuanghao11.cn

================================================================================
来源：http://yub.nwbrower.top

[J01] 获取当前时间
来源：http://tth.chenlongwang.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://kwm.ppjwa.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bwd.zdqjudy.top

JS:   new Date();  Date.now()
来源：http://gxo.ehwqpu.com

TS:   new Date();  Date.now()
来源：http://jzk.ehwqpu.com

Java: LocalDateTime.now();  Instant.now()
来源：http://etc.uphjek.com

Go:   time.Now()
来源：http://fls.tanke756.top

Ruby: Time.now
来源：http://bkt.hnqzz.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dhp.hongshengwenyu.top

[J02] 格式化输出
来源：http://eos.chenlongwang.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mnn.nanxinkj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://szk.jinqigfzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://owf.zhixingplan.top

TS:   d.toISOString()
来源：http://vzm.9152youxi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qyq.fanxiaobao.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tik.gotoacloud.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kol.vehdjk.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gph.jinqigufen.top

[J03] 字符串解析为日期
来源：http://dii.cdnleiting.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://woa.fanxiaobao.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://oxv.9152youxi.cn

JS:   new Date("2024-01-02")
来源：http://nzi.kuanghao11.cn

TS:   new Date("2024-01-02")
来源：http://caj.sxryk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jln.sufxvd.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://apd.hysaishi.cn

Ruby: Date.parse("2024-01-02")
来源：http://cpx.hcnkem.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://keg.hesvh.cn

[J04] 时间戳与日期互转
来源：http://vyy.chenjidiqi.icu

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ljn.nanxinkj.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rtl.bbcook.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tgw.uphjek.com

TS:   Math.floor(Date.now() / 1000)
来源：http://ibt.pycfn.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zmp.xingfuxueyuan.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hla.ctjpmb.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qjx.zdqjudy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ieo.hywenlv.cn

[J05] 时间加减（加 7 天）
来源：http://qvl.zhoulong.xyz

Py:   now + timedelta(days=7)
来源：http://mhr.daria6918.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zwf.smart0.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ulm.hesvh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bhn.xylfe.cn

Java: LocalDate.now().plusDays(7)
来源：http://nla.svipenyu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dfl.xinyue.icu

Ruby: Time.now + 7 * 86400
来源：http://iix.sysykeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://dnk.sufxvd.cn

[J06] 计算两时间之差
来源：http://agi.fanxiaobao.xyz

Py:   (end - start).total_seconds()
来源：http://fdk.pycfn.com

PHP:  $end->diff($start)->days;
来源：http://ein.xuanzx.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xjn.fzhhl.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lie.dashuyun.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bgp.zdbjq.cn

Go:   end.Sub(start).Hours()
来源：http://dgh.shzxlz.cn

Ruby: end - start                 # 返回秒数
来源：http://aga.kuanghao11.cn

C#:   (end - start).TotalSeconds
来源：http://ntl.9152youxi.cn

[J07] 比较两个日期
来源：http://ghb.vqdsnc.cn

Py:   d1 < d2;  d1 == d2
来源：http://klx.jqgfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vyd.jinqigufen.top

JS:   d1.getTime() < d2.getTime()
来源：http://xzw.zhiwuduotai.top

TS:   d1.getTime() < d2.getTime()
来源：http://wql.mhx1999.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ued.yanxiufei.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wbh.nwbrower.top

Ruby: d1 < d2;  d1 == d2
来源：http://qtg.shanyushiyangtech.top

C#:   d1 < d2;  d1 == d2
来源：http://qpz.aizwys.cn

[J08] 提取年月日与星期
来源：http://myc.jqgfzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hev.ppjwa.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ctc.yangfankeji.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ect.havefunace.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zld.birdmap.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fer.316326.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qau.hesvh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kgv.hnqzz.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dze.sufxvd.cn

[J09] 时区处理
来源：http://tnj.zhengqikj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xdz.jinqigufen.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://inr.xingfuxueyuan.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fbs.ctjpmb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zwh.cdnleiting.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vlv.jlsjyb.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://agt.sweek.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ocj.jqgfzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cjo.iojbl.cn

[J10] 取今天 / 本月第一天
来源：http://akz.cashguo.top

Py:   date.today();  date.today().replace(day=1)
来源：http://fsl.fzhhl.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xfg.daxiang520.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rxm.xinyue.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jwc.zhiwuduotai.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ptw.yfazqb.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pjz.bbcook.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pcm.jinyuanbaomall.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iec.havefunace.top

================================================================================
来源：http://qbk.jinqigfzy.top

K. JSON 与序列化
来源：http://pmd.cdnleiting.top

================================================================================
来源：http://vya.c1oappe.top

[K01] 对象转 JSON 字符串
来源：http://wci.jyoumei.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blx.jinqigfzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vod.jqgufenzy.top

JS:   JSON.stringify(obj)
来源：http://cok.kuanghao11.cn

TS:   JSON.stringify(obj)
来源：http://ljz.jinghuilouyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wcn.xinyue.icu

Go:   json.Marshal(obj)
来源：http://qte.yanxiufei.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mit.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://hwa.jinqigfzy.top

[K02] JSON 字符串转对象
来源：http://pdc.fzhhl.top

Py:   json.loads(s)
来源：http://fro.yuanzhike.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ooc.yvedp.cn

JS:   JSON.parse(s)
来源：http://unx.dianchejie.cn

TS:   JSON.parse(s)
来源：http://usk.zhiwuduotai.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://aki.ybcxt.top

Go:   json.Unmarshal(data, &v)
来源：http://lby.jqgfzy.top

Ruby: JSON.parse(s)
来源：http://joj.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hbu.ybcxt.top

[K03] JSON 美化输出（带缩进）
来源：http://kor.xingfuxueyuan.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kwy.jinqigfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bcn.hesvh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dfa.ctjpmb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://zgi.tarul.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uam.cucudq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wwo.hammf.cn

Ruby: JSON.pretty_generate(obj)
来源：http://aej.wangdashe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yus.zhiwuduotai.top

[K04] 读取 JSON 文件
来源：http://gsy.cucudq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zjc.gogol.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ptx.quarkkingdee.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kmz.iojbl.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://srv.nanxinkj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jsw.zycfv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://otj.birdmap.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://uhs.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ztn.shanyushiyangtech.top

[K05] 深拷贝对象
来源：http://mww.zycfv.cn

Py:   copy.deepcopy(obj)
来源：http://zop.aizwys.cn

PHP:  unserialize(serialize($obj));
来源：http://cxj.sysykeji.top

JS:   structuredClone(obj)
来源：http://smv.fzhhl.top

TS:   structuredClone(obj)
来源：http://gxf.sufxvd.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dvx.cashguo.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zdl.tarul.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uym.hnxiangtu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://mhq.guannengcc.top

[K06] 解析 URL 查询串
来源：http://ytg.cdnleiting.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xmy.shuidangran.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zbr.aizwys.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wea.nwbrower.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vbx.jinqigfzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://aon.yvedp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wje.yangfankeji.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pjz.yonumen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://quh.gotoacloud.top

[K07] 进制转换
来源：http://soa.wangdashe.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xyo.zhixingplan.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tmg.zhengqikj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lnv.zdbjq.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ixy.cdnleiting.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wxk.zhixingplan.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nqh.jinghuilouyu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wqv.jyoumei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qam.sjlbkw.cn

[K08] 二进制序列化（非 JSON）
来源：http://vrg.svipenyu.cn

Py:   pickle.dumps(obj)
来源：http://frc.yuanzhike.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wqz.shanyushiyangtech.top

JS:   v8.serialize(obj)        // Node
来源：http://uqf.uphjek.com

TS:   v8.serialize(obj)        // Node
来源：http://cwn.yonumen.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fgk.wangshuangyany.cn

Go:   encoding/gob
来源：http://nrv.dianchejie.cn

Ruby: Marshal.dump(obj)
来源：http://vgy.snrcjt.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ksw.hnxiangtu.top

================================================================================
来源：http://pzp.zhongyouzk.top

L. 网络请求
来源：http://rld.redwolf501.top

================================================================================
来源：http://amk.tarul.cn

[L01] 发送 GET 请求
来源：http://ciz.gzhubu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jvf.jinqigufen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uar.hnxiangtu.top

JS:   await fetch(url)
来源：http://pim.jinyuanbaomall.cn

TS:   await fetch(url)
来源：http://vty.chenlongwang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hrh.havefunace.top

Go:   resp, err := http.Get(url)
来源：http://bsj.bjfxy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://noe.yvedp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sby.cdnleiting.top

[L02] 发送 POST JSON
来源：http://dse.fengsongda.top

Py:   requests.post(url, json={"a": 1})
来源：http://hov.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xte.daxiang520.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://swa.iojbl.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://msa.zhiwuduotai.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ytz.tarul.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zon.jlsjyb.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gxx.shangyingyoupin.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hmz.yonumen.top

[L03] 设置自定义请求头
来源：http://tzj.yvedp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://udz.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vrk.c1oappe.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pil.jlsjyb.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vyr.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hur.zhiwuduotai.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xjy.uphjek.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rbc.yfazqb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sbd.ivvv.top

[L04] 设置超时
来源：http://pez.yj202588.top

Py:   requests.get(url, timeout=5)
来源：http://zai.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ner.zhiwuduotai.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jhx.tian-w.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://atg.jqgufenzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cef.zdqjudy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bkj.zhijiandao.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bpz.sweek.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fdx.jinghuilouyu.cn

[L05] 上传文件（multipart）
来源：http://ggs.yonumen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ncl.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zfz.sjlbkw.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xpl.cashguo.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qfp.uphjek.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hfl.aizwys.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yuo.ydzc1.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hfr.yvedp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wfw.hnxiangtu.top

[L06] 解析响应为 JSON
来源：http://cqv.xingfuxueyuan.xyz

Py:   resp.json()
来源：http://tdu.yangfankeji.com

PHP:  json_decode($body, true);
来源：http://xxg.smart0.xyz

JS:   await resp.json()
来源：http://api.fehbvm.com

TS:   await resp.json()
来源：http://cud.svipenyu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qlz.jyoumei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://frm.0kj1m.cn

Ruby: JSON.parse(resp.body)
来源：http://tyb.ydzc1.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://eez.jyoumei.cn

[L07] 处理 HTTP 状态码
来源：http://elh.fehbvm.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kzv.tian-w.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xhh.jianghu66.top

JS:   resp.ok;  resp.status
来源：http://xom.redwolf501.top


<!-- 参考信息 -->