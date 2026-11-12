代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lgh.zhongyouzk.top

PHP:  preg_match('/\d+/', $s);
来源：http://ijh.quarkkingdee.top

JS:   /\d+/.test(s)
来源：http://giv.0kj1m.cn

TS:   /\d+/.test(s)
来源：http://ugs.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vno.fzhhl.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pje.cheryme.top

Ruby: s.match?(/\d+/)
来源：http://rvm.daria6918.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sdb.ctjpmb.com

[I02] 提取所有匹配
来源：http://zvs.fengsongda.top

Py:   re.findall(r"\d+", s)
来源：http://xje.yvedp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yvb.nanxuanxn.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lhl.jqgufenzy.top

TS:   s.match(/\d+/g)
来源：http://eil.yj20258.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pff.yj20258888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://aqv.xziqi.cn

Ruby: s.scan(/\d+/)
来源：http://kuw.hnqzz.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://imo.sufxvd.cn

[I03] 提取捕获分组
来源：http://wyq.wangshuangyany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://enc.jianghu66.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zor.cdnleiting.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mbl.zhixingplan.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sly.wangshuangyany.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nyc.yuxming.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gck.hammf.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qdf.yongpay.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bec.hammf.cn

[I04] 正则替换
来源：http://syp.xuanzx.com

Py:   re.sub(r"\d+", "#", s)
来源：http://jql.redwolf501.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mbr.jqgfzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://lms.jinghuilouyu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xim.jqgfzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://jqd.xingfuxueyuan.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://ecq.daxiang520.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ajs.mhx1999.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ldp.jyoumei.cn

[I05] 按正则拆分
来源：http://joz.yanxiufei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pah.kuanghao11.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kpl.jinyuanbaomall.cn

JS:   s.split(/\s*,\s*/)
来源：http://sno.ydjk.org.cn

TS:   s.split(/\s*,\s*/)
来源：http://dta.kuanghao11.cn

Java: s.split("\\s*,\\s*")
来源：http://agj.yonumen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://alr.zhaomingkeji.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://pxv.yanxiufei.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xpu.ydjk.org.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yth.guannengcc.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yif.aizwys.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rqw.jinyuanbaomall.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qqz.hongshengwenyu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yfm.sysykeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bha.aizwys.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wfe.snrcjt.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qor.daria6918.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ded.zdbjq.cn

[I07] 忽略大小写与多行模式
来源：http://bdc.svipenyu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xiv.zdbjq.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://opx.zhaomingkeji.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bzg.gotoacloud.top

TS:   /error/gim
来源：http://zws.daria6918.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ybx.wangdashe.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nmz.hnqzz.top

Ruby: s.scan(/error/i)
来源：http://lcj.yonumen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qcs.316326.xyz

[I08] 贪婪与非贪婪匹配
来源：http://xgg.tarul.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sau.vqdsnc.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hnb.fehbvm.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kga.ivvv.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://slk.hnxiangtu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://lvz.epnwcf.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nuw.xylfe.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hwb.yfazqb.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tcs.zdqjudy.top

================================================================================
来源：http://xye.tian-w.cn

J. 日期与时间
来源：http://laz.yuanzhike.top

================================================================================
来源：http://egw.shuidangran.top

[J01] 获取当前时间
来源：http://elj.dianchejie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bfg.jqgfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yfu.wangdashe.top

JS:   new Date();  Date.now()
来源：http://ypx.hesvh.cn

TS:   new Date();  Date.now()
来源：http://vkq.quarkkingdee.top

Java: LocalDateTime.now();  Instant.now()
来源：http://zil.aibaodan.cn

Go:   time.Now()
来源：http://fuj.wangshuangyany.cn

Ruby: Time.now
来源：http://psp.dianchejie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uhs.xziqi.cn

[J02] 格式化输出
来源：http://lbn.ywan-chungtsiang.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zqb.gaohongyu789.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wpw.fktsv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iny.yj20258.top

TS:   d.toISOString()
来源：http://zlg.ydzc1.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bhc.hcnkem.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qhb.kuanghao11.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iqx.ywan-chungtsiang.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hxp.cdnleiting.top

[J03] 字符串解析为日期
来源：http://dam.ctjpmb.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rtn.yanxiufei.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hsx.ppjwa.cn

JS:   new Date("2024-01-02")
来源：http://nfw.jinghuilouyu.cn

TS:   new Date("2024-01-02")
来源：http://wei.smart0.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://esw.fzhhl.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lfz.zycfv.cn

Ruby: Date.parse("2024-01-02")
来源：http://lqq.fengsongda.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rkz.ctjpmb.com

[J04] 时间戳与日期互转
来源：http://phy.xziqi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vnc.0kj1m.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jos.jinqigufen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ndj.guowangkeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lgc.ppjwa.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://abg.vqdsnc.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lkg.hywenlv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gnp.cashguo.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xzo.svipenyu.cn

[J05] 时间加减（加 7 天）
来源：http://zzh.bbcook.cn

Py:   now + timedelta(days=7)
来源：http://dem.gotoacloud.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://oyo.chenlongwang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ghu.daxiang520.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://niq.yonumen.top

Java: LocalDate.now().plusDays(7)
来源：http://fnk.zdbjq.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lwl.zhoulong.xyz

Ruby: Time.now + 7 * 86400
来源：http://elc.hnxiangtu.top

C#:   DateTime.Now.AddDays(7)
来源：http://kua.vqdsnc.cn

[J06] 计算两时间之差
来源：http://ftd.sxryk.cn

Py:   (end - start).total_seconds()
来源：http://cnp.feifeiyinyue.top

PHP:  $end->diff($start)->days;
来源：http://rir.smart0.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bzd.cheryme.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lcm.daxiang520.top

Java: Duration.between(start, end).toSeconds()
来源：http://mjs.52xcode.cn

Go:   end.Sub(start).Hours()
来源：http://cem.jqgufenzy.top

Ruby: end - start                 # 返回秒数
来源：http://psq.hysaishi.cn

C#:   (end - start).TotalSeconds
来源：http://zab.fanxiaobao.xyz

[J07] 比较两个日期
来源：http://mgu.tian-w.cn

Py:   d1 < d2;  d1 == d2
来源：http://zpi.gogol.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cyn.xuetiantiany.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bbb.xziqi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://prt.cashguo.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://aaj.zhengqikj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rro.xingfuxueyuan.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://hns.yuanzhike.top

C#:   d1 < d2;  d1 == d2
来源：http://pms.aizwys.cn

[J08] 提取年月日与星期
来源：http://zzx.snrcjt.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dzv.ivvv.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ezm.fktsv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://efg.shanyushiyangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pns.shanyushiyangtech.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tve.iojbl.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mdn.sjlbkw.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pvw.hammf.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yam.ctjpmb.com

[J09] 时区处理
来源：http://zqm.mhx1999.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uee.sweek.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pii.xinyue.icu

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ett.andypj.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fjj.hnqzz.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wuf.ybcxt.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nod.sufxvd.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://oug.dianchejie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pex.hnxiangtu.top

[J10] 取今天 / 本月第一天
来源：http://dca.shzxlz.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ypd.tanke756.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://maq.cucudq.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://equ.c1oappe.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cuo.hysaishi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dqy.ydzc1.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://unk.meibo888.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://skg.bjfxy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ffa.xinyue.icu

================================================================================
来源：http://ywr.ydjk.org.cn

K. JSON 与序列化
来源：http://onu.daria6918.cn

================================================================================
来源：http://fic.ywan-chungtsiang.top

[K01] 对象转 JSON 字符串
来源：http://pxs.pycfn.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bja.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zpw.cucudq.cn

JS:   JSON.stringify(obj)
来源：http://ogs.hongshengwenyu.top

TS:   JSON.stringify(obj)
来源：http://qor.xinyue.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ywy.zhiwuduotai.top

Go:   json.Marshal(obj)
来源：http://fgf.xuetiantiany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://txe.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fte.ybcxt.top

[K02] JSON 字符串转对象
来源：http://zia.zhoulong.xyz

Py:   json.loads(s)
来源：http://yfm.hfpthk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://agj.hesvh.cn

JS:   JSON.parse(s)
来源：http://gcn.zhixingplan.top

TS:   JSON.parse(s)
来源：http://akc.hammf.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ccb.mhx1999.top

Go:   json.Unmarshal(data, &v)
来源：http://spn.gogol.net.cn

Ruby: JSON.parse(s)
来源：http://drx.tarul.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pjs.gzhubu.top

[K03] JSON 美化输出（带缩进）
来源：http://qcu.yj20258888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oql.wangshuangyany.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zip.jianghu66.top

JS:   JSON.stringify(obj, null, 2)
来源：http://fmp.hesvh.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xwm.dashuyun.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xbg.yuxming.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wiz.cucudq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ovr.dashuyun.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ssj.hammf.cn

[K04] 读取 JSON 文件
来源：http://umc.gogol.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nsn.zhengqikj.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://aqw.sweek.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qxw.birdmap.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uel.guannengcc.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://phc.ywan-chungtsiang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kur.gzhubu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://fqp.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://avc.dashuyun.cn

[K05] 深拷贝对象
来源：http://bvs.uphjek.com

Py:   copy.deepcopy(obj)
来源：http://rqk.yongpay.top

PHP:  unserialize(serialize($obj));
来源：http://bfn.jqgufenzy.top

JS:   structuredClone(obj)
来源：http://ovl.cashguo.top

TS:   structuredClone(obj)
来源：http://jiq.sysykeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ebb.nwbrower.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nmg.316326.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qjt.daxiang520.top

C#:   // 序列化往返，或自定义 Clone
来源：http://bbn.yuxming.cn

[K06] 解析 URL 查询串
来源：http://xgo.jinqigufen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://npr.yj202588.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://aox.yuxming.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nli.yongpay.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zlx.birdmap.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sgn.cqqwz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dxi.haohaochexian.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blz.meibo888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cej.fehbvm.com

[K07] 进制转换
来源：http://mzy.hongshengwenyu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zin.yuxming.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ljf.shanyushiyangkeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gcw.pengpengdd.cyou

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xpq.cheryme.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://loe.ctjpmb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pgq.fengsongda.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://doa.yanxiufei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cdm.yueranfly.top

[K08] 二进制序列化（非 JSON）
来源：http://rsy.ydzc1.top

Py:   pickle.dumps(obj)
来源：http://vdz.gotoacloud.top

PHP:  serialize($obj);  unserialize($s);
来源：http://rgq.hesvh.cn

JS:   v8.serialize(obj)        // Node
来源：http://vbo.shanyushiyangkeji.top

TS:   v8.serialize(obj)        // Node
来源：http://ybi.xylfe.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dik.yfazqb.com

Go:   encoding/gob
来源：http://xbt.ppjwa.cn

Ruby: Marshal.dump(obj)
来源：http://vzr.yuanzhike.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://drn.chenjidiqi.icu

================================================================================
来源：http://llx.tanke756.top

L. 网络请求
来源：http://zot.c1oappe.top

================================================================================
来源：http://tbm.smart0.xyz

[L01] 发送 GET 请求
来源：http://rut.meibo888.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://phf.yonumen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sgz.iojbl.cn

JS:   await fetch(url)
来源：http://nzk.ydjk.org.cn

TS:   await fetch(url)
来源：http://dwk.guowangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xhn.tianlin.xyz

Go:   resp, err := http.Get(url)
来源：http://ium.tian-w.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rto.haohaochexian.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jae.feifeiyinyue.top

[L02] 发送 POST JSON
来源：http://vvd.zhongyouzk.top

Py:   requests.post(url, json={"a": 1})
来源：http://tfk.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cwo.zhixingplan.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ybk.jinyuanbaomall.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://irc.hammf.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yrl.havefunace.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dkj.gzhubu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vkr.zhixingplan.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uit.fanxiaobao.xyz

[L03] 设置自定义请求头
来源：http://dzj.hfpthk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sjc.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ocy.zhixingplan.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uwl.52xcode.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://riz.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pua.fengsongda.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cly.yvedp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xhf.daxiang520.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ivz.smart0.xyz

[L04] 设置超时
来源：http://rno.cqqwz.cn

Py:   requests.get(url, timeout=5)
来源：http://zla.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ljz.shzxlz.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pol.ybcxt.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ofk.svipenyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mqd.cqqwz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fng.pycfn.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mxq.andypj.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gky.gogol.net.cn

[L05] 上传文件（multipart）
来源：http://pqu.jinqigufen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gbp.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://puo.316326.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wbt.52xcode.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hki.xinyue.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hea.cdnleiting.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rhl.guannengcc.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://aoh.sufxvd.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qpw.yuxming.cn

[L06] 解析响应为 JSON
来源：http://niz.ivvv.top

Py:   resp.json()
来源：http://rwz.vqdsnc.cn

PHP:  json_decode($body, true);
来源：http://oya.hnqzz.top

JS:   await resp.json()
来源：http://zoq.shanyushiyangkeji.top

TS:   await resp.json()
来源：http://pgh.jinqigfzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://plz.cashguo.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ary.fzhhl.top

Ruby: JSON.parse(resp.body)
来源：http://pal.tanke756.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ozu.yvedp.cn

[L07] 处理 HTTP 状态码
来源：http://fvo.yonumen.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rka.bjfxy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yvz.ivvv.top

JS:   resp.ok;  resp.status
来源：http://hhf.quarkkingdee.top


<!-- 参考信息 -->