代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oob.zhengqikj.top

PHP:  preg_match('/\d+/', $s);
来源：http://woy.gogol.net.cn

JS:   /\d+/.test(s)
来源：http://gwb.jlsjyb.cn

TS:   /\d+/.test(s)
来源：http://ngd.jinqigufen.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rwk.tian-w.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ysm.zhiwuduotai.top

Ruby: s.match?(/\d+/)
来源：http://had.fengsongda.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bco.kuanghao11.cn

[I02] 提取所有匹配
来源：http://sil.pengpengdd.cyou

Py:   re.findall(r"\d+", s)
来源：http://rys.yj20258.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hag.cashguo.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vpk.yangfankeji.com

TS:   s.match(/\d+/g)
来源：http://zrz.zhaomingkeji.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uqa.ivvv.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gje.sweek.top

Ruby: s.scan(/\d+/)
来源：http://cyt.epnwcf.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mwq.zycfv.cn

[I03] 提取捕获分组
来源：http://lyb.zhengqikj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ibw.jinqigfzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gyn.chenlongwang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://deb.hammf.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ais.yanxiufei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dvq.snrcjt.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://chh.hnqzz.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kfi.ywan-chungtsiang.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hid.ydzc1.top

[I04] 正则替换
来源：http://jae.0kj1m.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bky.epnwcf.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ssb.ydzc1.top

JS:   s.replace(/\d+/g, "#")
来源：http://chy.zhaomingkeji.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://wxd.ywan-chungtsiang.top

Java: s.replaceAll("\\d+", "#")
来源：http://fpr.chenlongwang.top

Go:   re.ReplaceAllString(s, "#")
来源：http://feq.fengsongda.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hyx.gotoacloud.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://oap.aibaodan.cn

[I05] 按正则拆分
来源：http://lya.jqgufenzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wer.pycfn.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sdj.ydzc1.top

JS:   s.split(/\s*,\s*/)
来源：http://jyl.zhoulong.xyz

TS:   s.split(/\s*,\s*/)
来源：http://ffg.guowangkeji.top

Java: s.split("\\s*,\\s*")
来源：http://bal.jinqigufen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ycy.jianghu66.top

Ruby: s.split(/\s*,\s*/)
来源：http://bor.cashguo.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ium.chenjidiqi.icu

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yny.epnwcf.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://svj.shangyingyoupin.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nab.ywan-chungtsiang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bba.ybcxt.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tfs.jinqigufen.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cel.havefunace.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eml.nanxuanxn.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ahc.iojbl.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hmy.yangfankeji.com

[I07] 忽略大小写与多行模式
来源：http://onu.smart0.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tdb.cqqwz.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ppk.hnqzz.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xaw.jyoumei.cn

TS:   /error/gim
来源：http://xkh.xuetiantiany.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cki.c1oappe.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qnw.zdqjudy.top

Ruby: s.scan(/error/i)
来源：http://ney.cqqwz.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ftw.pengpengdd.cyou

[I08] 贪婪与非贪婪匹配
来源：http://vvb.bbcook.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tvn.yj20258.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rlv.chenjidiqi.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xou.jlsjyb.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hjx.cucudq.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bfl.yuxming.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qdm.fktsv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dpi.cqqwz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dyj.hcnkem.com

================================================================================
来源：http://wrf.yj202588.top

J. 日期与时间
来源：http://lvc.zhaomingkeji.xyz

================================================================================
来源：http://vtp.vqdsnc.cn

[J01] 获取当前时间
来源：http://vis.sysykeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://rer.pengpengdd.cyou

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://suc.ybcxt.top

JS:   new Date();  Date.now()
来源：http://bry.ppjwa.cn

TS:   new Date();  Date.now()
来源：http://rfq.hfpthk.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lpi.cdnleiting.top

Go:   time.Now()
来源：http://rof.meibo888.top

Ruby: Time.now
来源：http://etc.wangshuangyany.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yzk.zdqjudy.top

[J02] 格式化输出
来源：http://twd.zhixingplan.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fpv.aibaodan.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qno.tian-w.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zfx.yj202588.top

TS:   d.toISOString()
来源：http://wtu.jinqigufen.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qix.yongpay.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nxy.zhijiandao.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://efc.52xcode.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vum.nwbrower.top

[J03] 字符串解析为日期
来源：http://clg.tian-w.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xqj.xuetiantiany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bno.shzxlz.cn

JS:   new Date("2024-01-02")
来源：http://iww.andypj.xyz

TS:   new Date("2024-01-02")
来源：http://sqt.guowangkeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://kms.jiagoushi.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fhd.ehwqpu.com

Ruby: Date.parse("2024-01-02")
来源：http://agv.nanxinkj.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uuc.fehbvm.com

[J04] 时间戳与日期互转
来源：http://ujt.redwolf501.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hqn.0kj1m.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dfu.yueranfly.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oyd.bbcook.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sgp.zhijiandao.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fqg.shanyushiyangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cko.zhaomingkeji.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ejw.sweek.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://izi.shanyushiyangtech.top

[J05] 时间加减（加 7 天）
来源：http://czt.epnwcf.com

Py:   now + timedelta(days=7)
来源：http://pkr.andypj.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://bjv.bbcook.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xuu.fehbvm.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jlc.birdmap.top

Java: LocalDate.now().plusDays(7)
来源：http://vtg.jinyuanbaomall.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uys.ywan-chungtsiang.top

Ruby: Time.now + 7 * 86400
来源：http://kkf.shuidangran.top

C#:   DateTime.Now.AddDays(7)
来源：http://kbn.sxryk.cn

[J06] 计算两时间之差
来源：http://szg.xziqi.cn

Py:   (end - start).total_seconds()
来源：http://cbd.fengsongda.top

PHP:  $end->diff($start)->days;
来源：http://qhp.jqgfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cql.hcnkem.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lbk.wangdashe.top

Java: Duration.between(start, end).toSeconds()
来源：http://fqh.xziqi.cn

Go:   end.Sub(start).Hours()
来源：http://jur.jinqigufen.top

Ruby: end - start                 # 返回秒数
来源：http://nvz.wangshuangyany.cn

C#:   (end - start).TotalSeconds
来源：http://tvk.yongpay.top

[J07] 比较两个日期
来源：http://lvq.zdqjudy.top

Py:   d1 < d2;  d1 == d2
来源：http://zqi.yj20258888.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qvc.fktsv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ptw.ctjpmb.com

TS:   d1.getTime() < d2.getTime()
来源：http://jtw.zdqjudy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hxe.fehbvm.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rvh.ppjwa.cn

Ruby: d1 < d2;  d1 == d2
来源：http://omd.haohaochexian.top

C#:   d1 < d2;  d1 == d2
来源：http://uib.sweek.top

[J08] 提取年月日与星期
来源：http://cdy.hywenlv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kat.ybcxt.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rij.xylfe.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zzz.nanxuanxn.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ajt.ivvv.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ywj.shangyingyoupin.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yig.redwolf501.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cet.ywan-chungtsiang.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ocz.shanyushiyangtech.top

[J09] 时区处理
来源：http://ufl.tian-w.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://loz.feifeiyinyue.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://klz.ydjk.org.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oxd.tarul.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ony.guannengcc.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hgy.ybcxt.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qbg.zhiwuduotai.top

Ruby: Time.now.getlocal("+08:00")
来源：http://krm.jinyuanbaomall.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rxw.fehbvm.com

[J10] 取今天 / 本月第一天
来源：http://pgr.ctjpmb.com

Py:   date.today();  date.today().replace(day=1)
来源：http://wzo.zhaomingkeji.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wnd.zhijiandao.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fll.fanxiaobao.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eif.fanxiaobao.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oso.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wwm.fanxiaobao.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fgi.zdbjq.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wxd.xylfe.cn

================================================================================
来源：http://icv.fzhhl.top

K. JSON 与序列化
来源：http://kir.jqgfzy.top

================================================================================
来源：http://gvs.ivvv.top

[K01] 对象转 JSON 字符串
来源：http://gup.fktsv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dcv.hongshengwenyu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cvk.daria6918.cn

JS:   JSON.stringify(obj)
来源：http://cpk.sjlbkw.cn

TS:   JSON.stringify(obj)
来源：http://vcw.52xcode.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nwh.ctjpmb.com

Go:   json.Marshal(obj)
来源：http://vqr.jinyuanbaomall.cn

Ruby: obj.to_json                                     // require "json"
来源：http://azv.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://unq.cheryme.top

[K02] JSON 字符串转对象
来源：http://cad.feifeiyinyue.top

Py:   json.loads(s)
来源：http://llw.nanxinkj.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cjz.tarul.cn

JS:   JSON.parse(s)
来源：http://eru.tianlin.xyz

TS:   JSON.parse(s)
来源：http://huq.daxiang520.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://geg.fzhhl.top

Go:   json.Unmarshal(data, &v)
来源：http://xfd.ydzc1.top

Ruby: JSON.parse(s)
来源：http://dsc.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tpr.jqgufenzy.top

[K03] JSON 美化输出（带缩进）
来源：http://tsj.yongpay.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fdd.xuetiantiany.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://itr.bbcook.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fgq.pengpengdd.cyou

TS:   JSON.stringify(obj, null, 2)
来源：http://vzd.chenlongwang.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ajp.gogol.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://naw.chenjidiqi.icu

Ruby: JSON.pretty_generate(obj)
来源：http://izg.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tky.shanyushiyangtech.top

[K04] 读取 JSON 文件
来源：http://mfx.zhengqikj.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ipc.nwbrower.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jpj.yonumen.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://koq.ctjpmb.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gaz.bbcook.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://amx.yuxming.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nmn.shuidangran.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://pwx.hesvh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://scd.uphjek.com

[K05] 深拷贝对象
来源：http://pep.guowangkeji.top

Py:   copy.deepcopy(obj)
来源：http://ypq.yuxming.cn

PHP:  unserialize(serialize($obj));
来源：http://yad.tarul.cn

JS:   structuredClone(obj)
来源：http://yri.xylfe.cn

TS:   structuredClone(obj)
来源：http://rpk.yfazqb.com

Java: // 手写拷贝构造，或序列化往返
来源：http://yob.jinqigfzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fyv.hcnkem.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qet.bbcook.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://atm.hammf.cn

[K06] 解析 URL 查询串
来源：http://lwt.jqgufenzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dqi.hcnkem.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wbj.bjfxy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pck.kuanghao11.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uut.feifeiyinyue.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ivx.shanyushiyangtech.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://oyr.hnqzz.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tgk.yonumen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ldt.xylfe.cn

[K07] 进制转换
来源：http://wqt.hfpthk.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zwm.zycfv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rqy.zhaomingkeji.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tix.sufxvd.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://svz.sxryk.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://etx.c1oappe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hat.fengsongda.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://msn.fanxiaobao.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rfp.yfazqb.com

[K08] 二进制序列化（非 JSON）
来源：http://psp.xuanzx.com

Py:   pickle.dumps(obj)
来源：http://itg.52xcode.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ven.guowangkeji.top

JS:   v8.serialize(obj)        // Node
来源：http://zgt.epnwcf.com

TS:   v8.serialize(obj)        // Node
来源：http://oby.sxryk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xzr.yuxming.cn

Go:   encoding/gob
来源：http://wqu.hammf.cn

Ruby: Marshal.dump(obj)
来源：http://anb.gotoacloud.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yee.zhongyouzk.top

================================================================================
来源：http://zxp.fanxiaobao.xyz

L. 网络请求
来源：http://grq.sxryk.cn

================================================================================
来源：http://jop.tanke756.top

[L01] 发送 GET 请求
来源：http://loa.bjfxy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://poa.jinqigufen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xcn.fktsv.cn

JS:   await fetch(url)
来源：http://alq.svipenyu.cn

TS:   await fetch(url)
来源：http://kjw.zycfv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tdp.zhaomingkeji.xyz

Go:   resp, err := http.Get(url)
来源：http://kbd.yonumen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://usp.yj20258.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pxn.gotoacloud.top

[L02] 发送 POST JSON
来源：http://ggm.316326.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://okv.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lcu.epnwcf.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cmc.nanxuanxn.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zki.ybcxt.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://utr.zhongyouzk.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aiw.zdqjudy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sch.uphjek.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ifi.sweek.top

[L03] 设置自定义请求头
来源：http://oyp.jyoumei.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rfc.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kyu.havefunace.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kli.yangfankeji.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ybj.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://igx.0kj1m.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jfj.redwolf501.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bph.havefunace.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ytn.meibo888.top

[L04] 设置超时
来源：http://xwi.jianghu66.top

Py:   requests.get(url, timeout=5)
来源：http://zpe.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://psc.pycfn.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qoh.iojbl.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ckn.ivvv.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nbm.shanyushiyangtech.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://amj.sysykeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rmw.ywan-chungtsiang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://psp.yanxiufei.cn

[L05] 上传文件（multipart）
来源：http://zhp.shanyushiyangtech.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xnw.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wlv.quarkkingdee.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ivu.meibo888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ght.guannengcc.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dcs.316326.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zcl.cheryme.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oka.sufxvd.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qth.tian-w.cn

[L06] 解析响应为 JSON
来源：http://xko.wangdashe.top

Py:   resp.json()
来源：http://lfp.chenjidiqi.icu

PHP:  json_decode($body, true);
来源：http://jno.andypj.xyz

JS:   await resp.json()
来源：http://swo.sufxvd.cn

TS:   await resp.json()
来源：http://bfd.hcnkem.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fke.ybcxt.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://toc.316326.xyz

Ruby: JSON.parse(resp.body)
来源：http://cej.xuetiantiany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sxx.yonumen.top

[L07] 处理 HTTP 状态码
来源：http://efv.c1oappe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tgp.ehwqpu.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zjo.vehdjk.com

JS:   resp.ok;  resp.status
来源：http://etp.andypj.xyz


<!-- 参考信息 -->