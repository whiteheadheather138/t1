代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vlh.xuanzx.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gmh.hnxiangtu.top

Ruby: s.match?(/\d+/)
来源：http://syl.zhongyouzk.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sbv.yj202588.top

[I02] 提取所有匹配
来源：http://qyu.wangshuangyany.cn

Py:   re.findall(r"\d+", s)
来源：http://ics.jiagoushi.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wvq.xylfe.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lko.havefunace.top

TS:   s.match(/\d+/g)
来源：http://ybw.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nyu.sjlbkw.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xex.52xcode.cn

Ruby: s.scan(/\d+/)
来源：http://var.yj20258.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://egb.pengpengdd.cyou

[I03] 提取捕获分组
来源：http://gns.daria6918.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ngc.zhaomingkeji.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fsx.jyoumei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oji.sjlbkw.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lob.fengsongda.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mnk.tanke756.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uqk.bbcook.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iwu.bjfxy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jtn.jinqigufen.top

[I04] 正则替换
来源：http://wwh.fengsongda.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jge.gaohongyu789.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cvh.nanxuanxn.top

JS:   s.replace(/\d+/g, "#")
来源：http://jvo.ywan-chungtsiang.top

TS:   s.replace(/\d+/g, "#")
来源：http://glf.yfazqb.com

Java: s.replaceAll("\\d+", "#")
来源：http://dnp.mhx1999.top

Go:   re.ReplaceAllString(s, "#")
来源：http://rsn.zhengqikj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ewt.nwbrower.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ycr.zhijiandao.cn

[I05] 按正则拆分
来源：http://gck.hnxiangtu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wba.shangyingyoupin.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://quj.shzxlz.cn

JS:   s.split(/\s*,\s*/)
来源：http://hik.jqgufenzy.top

TS:   s.split(/\s*,\s*/)
来源：http://fmv.xylfe.cn

Java: s.split("\\s*,\\s*")
来源：http://xvh.zhengqikj.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nkk.birdmap.top

Ruby: s.split(/\s*,\s*/)
来源：http://vkl.tianlin.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kon.sufxvd.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tpz.chenlongwang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xdn.chenzaomai.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://clp.nwbrower.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://byu.ctjpmb.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nim.sjlbkw.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blr.zhoulong.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lks.ydzc1.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ypk.sjlbkw.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://smb.hammf.cn

[I07] 忽略大小写与多行模式
来源：http://rmb.wangshuangyany.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cbx.guowangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sib.ybcxt.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jeu.shuidangran.top

TS:   /error/gim
来源：http://pkp.fzhhl.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yza.xylfe.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gkb.yuxming.cn

Ruby: s.scan(/error/i)
来源：http://wil.ydjk.org.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ncx.jiagoushi.top

[I08] 贪婪与非贪婪匹配
来源：http://zyg.ydzc1.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gcg.snrcjt.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hco.c1oappe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://svd.jqgfzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uxg.aibaodan.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yku.sufxvd.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nvo.jqgufenzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cju.epnwcf.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sxy.yj202588.top

================================================================================
来源：http://ain.sjlbkw.cn

J. 日期与时间
来源：http://gay.cdnleiting.top

================================================================================
来源：http://jgd.pycfn.com

[J01] 获取当前时间
来源：http://kzo.hcnkem.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://pjm.hnqzz.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ddi.hnxiangtu.top

JS:   new Date();  Date.now()
来源：http://gmq.yj202588.top

TS:   new Date();  Date.now()
来源：http://rbu.sjlbkw.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://iwd.nwbrower.top

Go:   time.Now()
来源：http://qhm.jinqigufen.top

Ruby: Time.now
来源：http://gxt.sufxvd.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sde.shzxlz.cn

[J02] 格式化输出
来源：http://qne.shzxlz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://egk.c1oappe.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iqw.cheryme.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lao.guowangkeji.top

TS:   d.toISOString()
来源：http://vqv.yuanzhike.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dwg.xziqi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rlx.kuanghao11.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xcn.jinqigfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://etz.iojbl.cn

[J03] 字符串解析为日期
来源：http://nzw.shuidangran.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jkx.yvedp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yyf.hesvh.cn

JS:   new Date("2024-01-02")
来源：http://fth.zhaomingkeji.xyz

TS:   new Date("2024-01-02")
来源：http://giv.wangdashe.top

Java: LocalDate.parse("2024-01-02")
来源：http://ddh.yueranfly.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bha.daria6918.cn

Ruby: Date.parse("2024-01-02")
来源：http://huk.nanxinkj.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dxi.wangshuangyany.cn

[J04] 时间戳与日期互转
来源：http://tlv.ivvv.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wnj.bbcook.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://efm.xuetiantiany.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hcv.hnqzz.top

TS:   Math.floor(Date.now() / 1000)
来源：http://eyb.316326.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nym.jinqigufen.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tyl.vqdsnc.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://imp.jqgfzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tvm.yuxming.cn

[J05] 时间加减（加 7 天）
来源：http://wvv.c1oappe.top

Py:   now + timedelta(days=7)
来源：http://nxd.pycfn.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://ezp.yj20258.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vqf.xylfe.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yvw.guannengcc.top

Java: LocalDate.now().plusDays(7)
来源：http://cdz.hcnkem.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uwh.jqgufenzy.top

Ruby: Time.now + 7 * 86400
来源：http://gbt.ydzc1.top

C#:   DateTime.Now.AddDays(7)
来源：http://wls.cucudq.cn

[J06] 计算两时间之差
来源：http://wvf.cqqwz.cn

Py:   (end - start).total_seconds()
来源：http://qvi.dianchejie.cn

PHP:  $end->diff($start)->days;
来源：http://jqs.hnqzz.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://waz.pycfn.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kzf.iojbl.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wwz.aizwys.cn

Go:   end.Sub(start).Hours()
来源：http://erl.tarul.cn

Ruby: end - start                 # 返回秒数
来源：http://ojs.tianlin.xyz

C#:   (end - start).TotalSeconds
来源：http://ouo.vqdsnc.cn

[J07] 比较两个日期
来源：http://kix.hfpthk.cn

Py:   d1 < d2;  d1 == d2
来源：http://ini.gzhubu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://iia.cheryme.top

JS:   d1.getTime() < d2.getTime()
来源：http://vwl.tian-w.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wwn.guannengcc.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pjq.sufxvd.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wrn.hcnkem.com

Ruby: d1 < d2;  d1 == d2
来源：http://uky.ywan-chungtsiang.top

C#:   d1 < d2;  d1 == d2
来源：http://kap.gaohongyu789.top

[J08] 提取年月日与星期
来源：http://nop.ppjwa.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://axy.jinqigfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mrp.hfpthk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uiw.shanyushiyangtech.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xra.jqgufenzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gug.xuanzx.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bqk.daxiang520.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vvg.tarul.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xbp.gogol.net.cn

[J09] 时区处理
来源：http://aop.bbcook.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ufl.ctjpmb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lul.shzxlz.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hir.vqdsnc.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://knk.zhijiandao.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jvr.yj202588.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://byf.jiagoushi.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vwi.yonumen.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://syj.xingfuxueyuan.xyz

[J10] 取今天 / 本月第一天
来源：http://iyy.jiagoushi.top

Py:   date.today();  date.today().replace(day=1)
来源：http://oyo.tianlin.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jmw.dashuyun.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pgr.c1oappe.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xzo.pycfn.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://iae.jiagoushi.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://glk.mhx1999.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kcr.hnxiangtu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tus.haohaochexian.top

================================================================================
来源：http://lof.aibaodan.cn

K. JSON 与序列化
来源：http://onp.jiagoushi.top

================================================================================
来源：http://ybj.xziqi.cn

[K01] 对象转 JSON 字符串
来源：http://mut.tian-w.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ade.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fft.iojbl.cn

JS:   JSON.stringify(obj)
来源：http://qyo.epnwcf.com

TS:   JSON.stringify(obj)
来源：http://qme.xinyue.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bev.jiagoushi.top

Go:   json.Marshal(obj)
来源：http://pjj.shangyingyoupin.top

Ruby: obj.to_json                                     // require "json"
来源：http://ejo.fzhhl.top

C#:   JsonSerializer.Serialize(obj)
来源：http://lme.xuetiantiany.cn

[K02] JSON 字符串转对象
来源：http://oir.sxryk.cn

Py:   json.loads(s)
来源：http://yea.fanxiaobao.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://maa.aizwys.cn

JS:   JSON.parse(s)
来源：http://tml.feifeiyinyue.top

TS:   JSON.parse(s)
来源：http://wra.316326.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jam.yanxiufei.cn

Go:   json.Unmarshal(data, &v)
来源：http://unz.ybcxt.top

Ruby: JSON.parse(s)
来源：http://fty.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tna.havefunace.top

[K03] JSON 美化输出（带缩进）
来源：http://qsq.sxryk.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://icn.jqgufenzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://aqg.cqqwz.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kcd.birdmap.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hsf.bjfxy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pns.yuxming.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mie.dianchejie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pme.zhixingplan.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nts.mhx1999.top

[K04] 读取 JSON 文件
来源：http://mhb.gzhubu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jmu.fktsv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wgx.sufxvd.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://clv.zhijiandao.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fec.hesvh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zla.redwolf501.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fao.tianlin.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://wif.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uxf.nanxuanxn.top

[K05] 深拷贝对象
来源：http://urb.jqgufenzy.top

Py:   copy.deepcopy(obj)
来源：http://btg.xylfe.cn

PHP:  unserialize(serialize($obj));
来源：http://yex.fzhhl.top

JS:   structuredClone(obj)
来源：http://rwk.nwbrower.top

TS:   structuredClone(obj)
来源：http://euj.shuidangran.top

Java: // 手写拷贝构造，或序列化往返
来源：http://eap.yanxiufei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ivp.ybcxt.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://led.ppjwa.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://psa.birdmap.top

[K06] 解析 URL 查询串
来源：http://tcw.jinghuilouyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pjs.jinghuilouyu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tro.uphjek.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eee.tanke756.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dgo.bjfxy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ycp.kuanghao11.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://clu.fehbvm.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kzt.yangfankeji.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://har.haohaochexian.top

[K07] 进制转换
来源：http://fiu.shangyingyoupin.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lkk.yongpay.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jpk.dashuyun.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iym.gaohongyu789.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jwt.dianchejie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qlc.tianlin.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://prd.ivvv.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gtd.vehdjk.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wvl.sweek.top

[K08] 二进制序列化（非 JSON）
来源：http://lez.gogol.net.cn

Py:   pickle.dumps(obj)
来源：http://djl.yj20258.top

PHP:  serialize($obj);  unserialize($s);
来源：http://fob.yangfankeji.com

JS:   v8.serialize(obj)        // Node
来源：http://ffm.andypj.xyz

TS:   v8.serialize(obj)        // Node
来源：http://kbs.cheryme.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ukd.ydjk.org.cn

Go:   encoding/gob
来源：http://alk.daria6918.cn

Ruby: Marshal.dump(obj)
来源：http://mqo.meibo888.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vtx.zhengqikj.top

================================================================================
来源：http://axx.hywenlv.cn

L. 网络请求
来源：http://hkn.svipenyu.cn

================================================================================
来源：http://uyd.chenjidiqi.icu

[L01] 发送 GET 请求
来源：http://bsg.ybcxt.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gul.yj20258888.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jbx.hcnkem.com

JS:   await fetch(url)
来源：http://wjv.xuetiantiany.cn

TS:   await fetch(url)
来源：http://eju.havefunace.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mug.yj20258.top

Go:   resp, err := http.Get(url)
来源：http://mzp.fehbvm.com

Ruby: Net::HTTP.get(URI(url))
来源：http://qzx.sufxvd.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sun.aizwys.cn

[L02] 发送 POST JSON
来源：http://koc.fehbvm.com

Py:   requests.post(url, json={"a": 1})
来源：http://gmj.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pme.yvedp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rqv.sxryk.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://phq.redwolf501.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dny.cashguo.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kmf.havefunace.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vlt.meibo888.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qwn.52xcode.cn

[L03] 设置自定义请求头
来源：http://ruv.nanxinkj.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://svj.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jwz.fanxiaobao.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tmq.gaohongyu789.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tfl.zdbjq.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cyj.ydjk.org.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bnv.zhixingplan.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oow.bjfxy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://msa.zhoulong.xyz

[L04] 设置超时
来源：http://ouh.daria6918.cn

Py:   requests.get(url, timeout=5)
来源：http://apb.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://glf.zycfv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zfm.epnwcf.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zev.fehbvm.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cjp.zhijiandao.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pks.xziqi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lxx.uphjek.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://spx.cashguo.top

[L05] 上传文件（multipart）
来源：http://mup.ydjk.org.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yml.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://new.quarkkingdee.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lsj.xylfe.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kue.ybcxt.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vot.epnwcf.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nma.chenlongwang.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wmx.zdbjq.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ugz.cqqwz.cn

[L06] 解析响应为 JSON
来源：http://zxo.wangshuangyany.cn

Py:   resp.json()
来源：http://rdb.yangfankeji.com

PHP:  json_decode($body, true);
来源：http://wou.c1oappe.top

JS:   await resp.json()
来源：http://chj.guannengcc.top

TS:   await resp.json()
来源：http://rzr.snrcjt.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ywr.nwbrower.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hdk.zdbjq.cn

Ruby: JSON.parse(resp.body)
来源：http://skt.hcnkem.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iht.bjfxy.top

[L07] 处理 HTTP 状态码
来源：http://chw.aibaodan.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://usb.chenzaomai.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zph.shuidangran.top

JS:   resp.ok;  resp.status
来源：http://wms.svipenyu.cn

TS:   resp.ok;  resp.status
来源：http://pvj.shanyushiyangkeji.top

Java: resp.statusCode()
来源：http://vou.wangdashe.top

Go:   resp.StatusCode
来源：http://vma.gotoacloud.top

Ruby: resp.code.to_i
来源：http://pmu.yvedp.cn


<!-- 参考信息 -->