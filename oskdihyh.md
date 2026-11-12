代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bol.xylfe.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kwe.haohaochexian.top

Ruby: s.match?(/\d+/)
来源：http://iol.hnqzz.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pvr.sjlbkw.cn

[I02] 提取所有匹配
来源：http://lsx.jinqigfzy.top

Py:   re.findall(r"\d+", s)
来源：http://qpz.cdnleiting.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ziq.bjfxy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jbr.ctjpmb.com

TS:   s.match(/\d+/g)
来源：http://hbm.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mrg.yongpay.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kal.shzxlz.cn

Ruby: s.scan(/\d+/)
来源：http://vqz.yangfankeji.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ksu.fanxiaobao.xyz

[I03] 提取捕获分组
来源：http://jaw.jyoumei.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://slg.pengpengdd.cyou

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cjz.wangdashe.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ast.sweek.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kkz.ivvv.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oux.epnwcf.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pro.feifeiyinyue.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vcm.daxiang520.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sxx.chenlongwang.top

[I04] 正则替换
来源：http://skh.hywenlv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://iii.sweek.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cvn.fehbvm.com

JS:   s.replace(/\d+/g, "#")
来源：http://nwm.nanxinkj.top

TS:   s.replace(/\d+/g, "#")
来源：http://aoa.smart0.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://imv.wangshuangyany.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ypj.ehwqpu.com

Ruby: s.gsub(/\d+/, "#")
来源：http://btc.c1oappe.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wbq.shuidangran.top

[I05] 按正则拆分
来源：http://hqn.nwbrower.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hwk.jlsjyb.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jfk.wangshuangyany.cn

JS:   s.split(/\s*,\s*/)
来源：http://klb.jiagoushi.top

TS:   s.split(/\s*,\s*/)
来源：http://yce.yuxming.cn

Java: s.split("\\s*,\\s*")
来源：http://ibh.hammf.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://aoz.zhoulong.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://qmp.pengpengdd.cyou

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fgt.shanyushiyangtech.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vro.quarkkingdee.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dea.pengpengdd.cyou

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mxd.ydjk.org.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vmb.nanxuanxn.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pdx.zdbjq.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ylg.zdqjudy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cog.birdmap.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mzd.fengsongda.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qkk.9152youxi.cn

[I07] 忽略大小写与多行模式
来源：http://srn.shzxlz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fuz.jinghuilouyu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xgz.ivvv.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ylf.iojbl.cn

TS:   /error/gim
来源：http://kji.tanke756.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wou.hywenlv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gty.feifeiyinyue.top

Ruby: s.scan(/error/i)
来源：http://mtx.sweek.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rhb.smart0.xyz

[I08] 贪婪与非贪婪匹配
来源：http://mfp.cqqwz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://chq.cqqwz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dre.yongpay.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://keh.nwbrower.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rfy.gzhubu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://gde.nanxuanxn.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fwg.shanyushiyangkeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jfk.jlsjyb.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ksg.quarkkingdee.top

================================================================================
来源：http://xzp.jianghu66.top

J. 日期与时间
来源：http://yqp.jinghuilouyu.cn

================================================================================
来源：http://gph.xylfe.cn

[J01] 获取当前时间
来源：http://jhk.pycfn.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://fof.hnqzz.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uwp.zhiwuduotai.top

JS:   new Date();  Date.now()
来源：http://sni.pycfn.com

TS:   new Date();  Date.now()
来源：http://kxs.hammf.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ilk.hammf.cn

Go:   time.Now()
来源：http://nml.cashguo.top

Ruby: Time.now
来源：http://yst.fktsv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lji.hysaishi.cn

[J02] 格式化输出
来源：http://ezj.c1oappe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kln.aibaodan.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qwk.quarkkingdee.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://btl.tian-w.cn

TS:   d.toISOString()
来源：http://rcf.xuanzx.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dws.shzxlz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://eiw.xuetiantiany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ulj.zhaomingkeji.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gah.ydzc1.top

[J03] 字符串解析为日期
来源：http://tbx.uphjek.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pzk.hongshengwenyu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qrx.sufxvd.cn

JS:   new Date("2024-01-02")
来源：http://rrk.yuxming.cn

TS:   new Date("2024-01-02")
来源：http://ats.ehwqpu.com

Java: LocalDate.parse("2024-01-02")
来源：http://dfk.gogol.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://juc.jianghu66.top

Ruby: Date.parse("2024-01-02")
来源：http://snv.vqdsnc.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mvi.yuxming.cn

[J04] 时间戳与日期互转
来源：http://xpz.shanyushiyangtech.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mnf.fktsv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://koy.zhijiandao.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iwi.jinqigufen.top

TS:   Math.floor(Date.now() / 1000)
来源：http://igb.havefunace.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://djx.wangdashe.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://joi.shanyushiyangtech.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://soj.havefunace.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sod.birdmap.top

[J05] 时间加减（加 7 天）
来源：http://gvs.sysykeji.top

Py:   now + timedelta(days=7)
来源：http://gsd.gzhubu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qhu.jinghuilouyu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lpo.hongshengwenyu.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wyy.yj20258.top

Java: LocalDate.now().plusDays(7)
来源：http://bxl.yfazqb.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://abn.hywenlv.cn

Ruby: Time.now + 7 * 86400
来源：http://mfp.iojbl.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pgd.fanxiaobao.xyz

[J06] 计算两时间之差
来源：http://wvu.smart0.xyz

Py:   (end - start).total_seconds()
来源：http://ead.hnxiangtu.top

PHP:  $end->diff($start)->days;
来源：http://fki.birdmap.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://seu.yj20258888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rdh.snrcjt.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cef.feifeiyinyue.top

Go:   end.Sub(start).Hours()
来源：http://pvp.hnqzz.top

Ruby: end - start                 # 返回秒数
来源：http://ieu.yuanzhike.top

C#:   (end - start).TotalSeconds
来源：http://fxd.yfazqb.com

[J07] 比较两个日期
来源：http://zjq.kuanghao11.cn

Py:   d1 < d2;  d1 == d2
来源：http://wsr.jqgfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://caq.hongshengwenyu.top

JS:   d1.getTime() < d2.getTime()
来源：http://ain.52xcode.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ryl.ybcxt.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bsv.yj20258888.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://che.zhijiandao.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vze.jinqigufen.top

C#:   d1 < d2;  d1 == d2
来源：http://qdu.iojbl.cn

[J08] 提取年月日与星期
来源：http://abd.cucudq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ijg.fktsv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tst.yvedp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://shu.snrcjt.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pkc.xziqi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ifm.gotoacloud.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://znk.uphjek.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vqw.quarkkingdee.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://irk.zhiwuduotai.top

[J09] 时区处理
来源：http://ufb.cdnleiting.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gaq.hesvh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wgb.tarul.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kcu.jianghu66.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rnt.dashuyun.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oqn.daxiang520.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vcq.yongpay.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vnr.aibaodan.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jqe.zhixingplan.top

[J10] 取今天 / 本月第一天
来源：http://fif.ppjwa.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hqy.zdqjudy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yvg.snrcjt.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gik.yj202588.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xzb.ywan-chungtsiang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kai.yvedp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://siv.yuxming.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wbk.cucudq.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qlq.yonumen.top

================================================================================
来源：http://qap.jiagoushi.top

K. JSON 与序列化
来源：http://ztg.svipenyu.cn

================================================================================
来源：http://wmk.shuidangran.top

[K01] 对象转 JSON 字符串
来源：http://xtn.shanyushiyangtech.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cjx.tianlin.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wkc.316326.xyz

JS:   JSON.stringify(obj)
来源：http://kxj.shanyushiyangkeji.top

TS:   JSON.stringify(obj)
来源：http://wpn.tanke756.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lnk.yongpay.top

Go:   json.Marshal(obj)
来源：http://ovd.ywan-chungtsiang.top

Ruby: obj.to_json                                     // require "json"
来源：http://mhk.hammf.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://men.jiagoushi.top

[K02] JSON 字符串转对象
来源：http://ths.yj20258888.top

Py:   json.loads(s)
来源：http://krr.yanxiufei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dar.shanyushiyangtech.top

JS:   JSON.parse(s)
来源：http://wfm.gotoacloud.top

TS:   JSON.parse(s)
来源：http://zlx.smart0.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qhm.xylfe.cn

Go:   json.Unmarshal(data, &v)
来源：http://toc.c1oappe.top

Ruby: JSON.parse(s)
来源：http://qqq.nanxuanxn.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://apo.jinyuanbaomall.cn

[K03] JSON 美化输出（带缩进）
来源：http://grp.cashguo.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ynx.chenlongwang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wbr.hfpthk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gau.sweek.top

TS:   JSON.stringify(obj, null, 2)
来源：http://cps.yuanzhike.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zck.cqqwz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bry.meibo888.top

Ruby: JSON.pretty_generate(obj)
来源：http://mzt.svipenyu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gkx.sweek.top

[K04] 读取 JSON 文件
来源：http://pko.guowangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lhw.ppjwa.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://njg.c1oappe.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yqg.zdqjudy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vcx.jqgufenzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xrs.vqdsnc.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sar.yangfankeji.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://pwm.uphjek.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jfj.nanxinkj.top

[K05] 深拷贝对象
来源：http://gee.nwbrower.top

Py:   copy.deepcopy(obj)
来源：http://bkn.dashuyun.cn

PHP:  unserialize(serialize($obj));
来源：http://kld.jianghu66.top

JS:   structuredClone(obj)
来源：http://nbz.birdmap.top

TS:   structuredClone(obj)
来源：http://fjk.mhx1999.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ayl.feifeiyinyue.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ndp.jinyuanbaomall.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kqk.zhiwuduotai.top

C#:   // 序列化往返，或自定义 Clone
来源：http://izw.xingfuxueyuan.xyz

[K06] 解析 URL 查询串
来源：http://qgd.yvedp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fbl.jqgfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hvp.daxiang520.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hzp.hongshengwenyu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rjg.zhixingplan.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gxg.shzxlz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://urn.chenlongwang.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cvt.xziqi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zkk.chenzaomai.com

[K07] 进制转换
来源：http://bna.yj202588.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fkm.gotoacloud.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fhc.zhixingplan.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bqy.gaohongyu789.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hry.zhengqikj.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zjq.zycfv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://puv.feifeiyinyue.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mor.fktsv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nff.jlsjyb.cn

[K08] 二进制序列化（非 JSON）
来源：http://fxp.chenzaomai.com

Py:   pickle.dumps(obj)
来源：http://vzm.jinghuilouyu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zoi.tian-w.cn

JS:   v8.serialize(obj)        // Node
来源：http://fft.sxryk.cn

TS:   v8.serialize(obj)        // Node
来源：http://qyt.cashguo.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gvl.zhongyouzk.top

Go:   encoding/gob
来源：http://hur.xinyue.icu

Ruby: Marshal.dump(obj)
来源：http://bwf.meibo888.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uuq.zhongyouzk.top

================================================================================
来源：http://nvf.hammf.cn

L. 网络请求
来源：http://ejj.zhengqikj.top

================================================================================
来源：http://mkl.52xcode.cn

[L01] 发送 GET 请求
来源：http://fok.nanxuanxn.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://top.iojbl.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lpc.guannengcc.top

JS:   await fetch(url)
来源：http://pic.gzhubu.top

TS:   await fetch(url)
来源：http://gsk.redwolf501.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sqa.yj202588.top

Go:   resp, err := http.Get(url)
来源：http://yip.fzhhl.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dcw.hongshengwenyu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vgd.andypj.xyz

[L02] 发送 POST JSON
来源：http://tfq.havefunace.top

Py:   requests.post(url, json={"a": 1})
来源：http://bdv.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kvf.uphjek.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uqu.xuetiantiany.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hqf.fanxiaobao.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://amr.yj202588.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hyr.jiagoushi.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pfn.hywenlv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xft.chenzaomai.com

[L03] 设置自定义请求头
来源：http://grq.316326.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://luq.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bje.ybcxt.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hfq.ppjwa.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://klr.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cco.birdmap.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zxf.bjfxy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://luh.birdmap.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mjr.ivvv.top

[L04] 设置超时
来源：http://lqp.cdnleiting.top

Py:   requests.get(url, timeout=5)
来源：http://ciz.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qzf.jinqigfzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jbi.zhaomingkeji.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zho.zhijiandao.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wcn.shuidangran.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sbi.uphjek.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vvs.epnwcf.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jhl.xuanzx.com

[L05] 上传文件（multipart）
来源：http://knf.sxryk.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nti.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nog.gaohongyu789.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dsm.zhaomingkeji.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gpe.fzhhl.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gio.sysykeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wyc.jqgufenzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://utw.yvedp.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eyv.316326.xyz

[L06] 解析响应为 JSON
来源：http://yvo.daria6918.cn

Py:   resp.json()
来源：http://cfn.chenlongwang.top

PHP:  json_decode($body, true);
来源：http://xoz.c1oappe.top

JS:   await resp.json()
来源：http://tkl.316326.xyz

TS:   await resp.json()
来源：http://ioe.gogol.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pwd.ydjk.org.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://avq.jinghuilouyu.cn

Ruby: JSON.parse(resp.body)
来源：http://pfh.yj20258.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hnr.wangdashe.top

[L07] 处理 HTTP 状态码
来源：http://bbd.vehdjk.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rzg.zhaomingkeji.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jma.pengpengdd.cyou

JS:   resp.ok;  resp.status
来源：http://jab.tarul.cn

TS:   resp.ok;  resp.status
来源：http://vql.hammf.cn

Java: resp.statusCode()
来源：http://rqv.jinqigufen.top

Go:   resp.StatusCode
来源：http://iii.jiagoushi.top

Ruby: resp.code.to_i
来源：http://cff.dianchejie.cn


<!-- 参考信息 -->