代发 wailian999

================================================================================
来源：http://ces.yangfankeji.com

I. 正则表达式
来源：http://utm.zhijiandao.cn

================================================================================
来源：http://diw.shzxlz.cn

[I01] 判断是否匹配
来源：http://jtx.yonumen.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rvq.jinghuilouyu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://igl.gaohongyu789.top

JS:   /\d+/.test(s)
来源：http://lte.quarkkingdee.top

TS:   /\d+/.test(s)
来源：http://ofw.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ecx.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jik.shanyushiyangtech.top

Ruby: s.match?(/\d+/)
来源：http://sar.316326.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hov.gaohongyu789.top

[I02] 提取所有匹配
来源：http://wrc.c1oappe.top

Py:   re.findall(r"\d+", s)
来源：http://kzw.xingfuxueyuan.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xfc.ybcxt.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xxe.jinqigfzy.top

TS:   s.match(/\d+/g)
来源：http://kxy.zhaomingkeji.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kzc.aibaodan.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://obd.hfpthk.cn

Ruby: s.scan(/\d+/)
来源：http://bqs.sweek.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nkl.hnxiangtu.top

[I03] 提取捕获分组
来源：http://zym.zhaomingkeji.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xai.cheryme.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ybr.sufxvd.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mzw.pycfn.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hrf.xziqi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xwe.zycfv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vdv.jqgfzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wff.nanxuanxn.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://few.fehbvm.com

[I04] 正则替换
来源：http://hsi.uphjek.com

Py:   re.sub(r"\d+", "#", s)
来源：http://pfs.guannengcc.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vrd.jqgfzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://hbu.sysykeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://fui.ydjk.org.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lvx.zhiwuduotai.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qkl.nanxinkj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hrw.zhiwuduotai.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tuq.chenzaomai.com

[I05] 按正则拆分
来源：http://kff.gogol.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hqf.fktsv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lxn.hywenlv.cn

JS:   s.split(/\s*,\s*/)
来源：http://ygn.jinqigufen.top

TS:   s.split(/\s*,\s*/)
来源：http://ger.yfazqb.com

Java: s.split("\\s*,\\s*")
来源：http://xav.hnqzz.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gzi.hfpthk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sip.shanyushiyangtech.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://shf.yj20258.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rnt.meibo888.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gtm.52xcode.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pod.aizwys.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nsz.chenlongwang.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qac.dashuyun.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wau.bbcook.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jrn.yj202588.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jrm.dashuyun.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://iwo.xuanzx.com

[I07] 忽略大小写与多行模式
来源：http://rud.hcnkem.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zaj.yfazqb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://znp.jiagoushi.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cib.shangyingyoupin.top

TS:   /error/gim
来源：http://bvj.yangfankeji.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pwj.snrcjt.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kwb.meibo888.top

Ruby: s.scan(/error/i)
来源：http://gdl.ybcxt.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ioc.cucudq.cn

[I08] 贪婪与非贪婪匹配
来源：http://fzm.andypj.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rjh.shanyushiyangkeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tvq.tianlin.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dou.zhixingplan.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nze.sweek.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://gxa.epnwcf.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dva.hysaishi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kka.hywenlv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fiw.daxiang520.top

================================================================================
来源：http://arr.zhixingplan.top

J. 日期与时间
来源：http://izm.feifeiyinyue.top

================================================================================
来源：http://yhn.hongshengwenyu.top

[J01] 获取当前时间
来源：http://yrp.pengpengdd.cyou

Py:   datetime.now();  datetime.now(UTC)
来源：http://arz.jqgufenzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yff.hysaishi.cn

JS:   new Date();  Date.now()
来源：http://euj.zdbjq.cn

TS:   new Date();  Date.now()
来源：http://zhh.pycfn.com

Java: LocalDateTime.now();  Instant.now()
来源：http://gnh.aibaodan.cn

Go:   time.Now()
来源：http://bgr.iojbl.cn

Ruby: Time.now
来源：http://fsu.shangyingyoupin.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zyc.nanxuanxn.top

[J02] 格式化输出
来源：http://zhx.yangfankeji.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xmc.ydzc1.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bjx.tianlin.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wtf.yongpay.top

TS:   d.toISOString()
来源：http://xwh.andypj.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vbc.yfazqb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hqd.hnqzz.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tnq.shzxlz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jkz.hesvh.cn

[J03] 字符串解析为日期
来源：http://ohz.shanyushiyangtech.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pyw.quarkkingdee.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dry.gogol.net.cn

JS:   new Date("2024-01-02")
来源：http://tve.zdbjq.cn

TS:   new Date("2024-01-02")
来源：http://mqy.nanxinkj.top

Java: LocalDate.parse("2024-01-02")
来源：http://ogb.dashuyun.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://igp.gaohongyu789.top

Ruby: Date.parse("2024-01-02")
来源：http://vei.aibaodan.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://iwb.aizwys.cn

[J04] 时间戳与日期互转
来源：http://kon.uphjek.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sxl.chenlongwang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cib.shanyushiyangkeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qmd.birdmap.top

TS:   Math.floor(Date.now() / 1000)
来源：http://oxa.ppjwa.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jsx.gotoacloud.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oor.daria6918.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://onj.xziqi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mld.hongshengwenyu.top

[J05] 时间加减（加 7 天）
来源：http://dxw.zycfv.cn

Py:   now + timedelta(days=7)
来源：http://ydc.yvedp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cmn.chenzaomai.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://juq.hcnkem.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tjs.hesvh.cn

Java: LocalDate.now().plusDays(7)
来源：http://frd.chenjidiqi.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://giw.shuidangran.top

Ruby: Time.now + 7 * 86400
来源：http://shd.aibaodan.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ljy.wangshuangyany.cn

[J06] 计算两时间之差
来源：http://hqp.aizwys.cn

Py:   (end - start).total_seconds()
来源：http://koa.tian-w.cn

PHP:  $end->diff($start)->days;
来源：http://bdk.316326.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eqi.pengpengdd.cyou

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sqr.zhoulong.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://nnr.birdmap.top

Go:   end.Sub(start).Hours()
来源：http://vdu.cdnleiting.top

Ruby: end - start                 # 返回秒数
来源：http://ixk.xingfuxueyuan.xyz

C#:   (end - start).TotalSeconds
来源：http://yna.jlsjyb.cn

[J07] 比较两个日期
来源：http://loh.pengpengdd.cyou

Py:   d1 < d2;  d1 == d2
来源：http://dpq.gaohongyu789.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hmw.gotoacloud.top

JS:   d1.getTime() < d2.getTime()
来源：http://ebi.9152youxi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gvi.yonumen.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ckk.dianchejie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ptr.andypj.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://fue.cucudq.cn

C#:   d1 < d2;  d1 == d2
来源：http://bou.ppjwa.cn

[J08] 提取年月日与星期
来源：http://zvc.c1oappe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pax.smart0.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ekd.jqgfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gjb.wangshuangyany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://avv.jinghuilouyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://icr.hysaishi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jwb.zhoulong.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vgm.snrcjt.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xft.guannengcc.top

[J09] 时区处理
来源：http://aou.jianghu66.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gpq.tianlin.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sww.pengpengdd.cyou

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pzx.hywenlv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gic.zhaomingkeji.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rzg.gaohongyu789.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://djb.zhengqikj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bhk.aizwys.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vfm.guannengcc.top

[J10] 取今天 / 本月第一天
来源：http://akw.xuanzx.com

Py:   date.today();  date.today().replace(day=1)
来源：http://uvh.nwbrower.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tva.yvedp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hmd.jiagoushi.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gjj.zhiwuduotai.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://evo.haohaochexian.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gwk.chenjidiqi.icu

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://aoo.yj20258.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jji.sxryk.cn

================================================================================
来源：http://pyt.vehdjk.com

K. JSON 与序列化
来源：http://msj.hammf.cn

================================================================================
来源：http://bsd.haohaochexian.top

[K01] 对象转 JSON 字符串
来源：http://jqy.xuetiantiany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://afu.chenlongwang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ono.aizwys.cn

JS:   JSON.stringify(obj)
来源：http://ejy.jianghu66.top

TS:   JSON.stringify(obj)
来源：http://dbj.tian-w.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nup.gotoacloud.top

Go:   json.Marshal(obj)
来源：http://sxe.snrcjt.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cvp.zhixingplan.top

C#:   JsonSerializer.Serialize(obj)
来源：http://mqg.wangshuangyany.cn

[K02] JSON 字符串转对象
来源：http://eys.jinyuanbaomall.cn

Py:   json.loads(s)
来源：http://cvk.jyoumei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oik.jqgufenzy.top

JS:   JSON.parse(s)
来源：http://ljt.jinqigfzy.top

TS:   JSON.parse(s)
来源：http://cpf.jinghuilouyu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pbc.yuanzhike.top

Go:   json.Unmarshal(data, &v)
来源：http://jul.wangshuangyany.cn

Ruby: JSON.parse(s)
来源：http://kye.svipenyu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mja.fzhhl.top

[K03] JSON 美化输出（带缩进）
来源：http://wpi.chenzaomai.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hkn.yj202588.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mjv.tanke756.top

JS:   JSON.stringify(obj, null, 2)
来源：http://oru.yvedp.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dbr.yongpay.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qui.ctjpmb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qgk.zdqjudy.top

Ruby: JSON.pretty_generate(obj)
来源：http://tbv.jqgfzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jhs.aibaodan.cn

[K04] 读取 JSON 文件
来源：http://aoy.gaohongyu789.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zkm.hcnkem.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nbu.dashuyun.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://faw.shanyushiyangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mfs.ydzc1.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nlu.chenlongwang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pmz.uphjek.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://xxc.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dno.tianlin.xyz

[K05] 深拷贝对象
来源：http://wou.cheryme.top

Py:   copy.deepcopy(obj)
来源：http://cnc.0kj1m.cn

PHP:  unserialize(serialize($obj));
来源：http://cmy.hywenlv.cn

JS:   structuredClone(obj)
来源：http://kkn.ivvv.top

TS:   structuredClone(obj)
来源：http://adr.sweek.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bff.jinghuilouyu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tdy.hammf.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ktl.xingfuxueyuan.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://hhp.vqdsnc.cn

[K06] 解析 URL 查询串
来源：http://zdo.yj202588.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://drk.shanyushiyangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pjk.zhengqikj.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nbu.yuxming.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gxm.vehdjk.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pfa.epnwcf.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://oiv.snrcjt.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://crb.smart0.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vim.ppjwa.cn

[K07] 进制转换
来源：http://prn.fzhhl.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hiv.pycfn.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zgn.hnqzz.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yii.yangfankeji.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ptg.hesvh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://arm.fanxiaobao.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ziw.zhijiandao.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fid.yanxiufei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tfm.aibaodan.cn

[K08] 二进制序列化（非 JSON）
来源：http://jjy.cucudq.cn

Py:   pickle.dumps(obj)
来源：http://wtl.nanxuanxn.top

PHP:  serialize($obj);  unserialize($s);
来源：http://drr.ybcxt.top

JS:   v8.serialize(obj)        // Node
来源：http://kse.xingfuxueyuan.xyz

TS:   v8.serialize(obj)        // Node
来源：http://gtk.meibo888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wvt.hesvh.cn

Go:   encoding/gob
来源：http://log.nwbrower.top

Ruby: Marshal.dump(obj)
来源：http://ypi.zhaomingkeji.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kio.xinyue.icu

================================================================================
来源：http://ykx.hfpthk.cn

L. 网络请求
来源：http://cvy.guowangkeji.top

================================================================================
来源：http://nrh.dianchejie.cn

[L01] 发送 GET 请求
来源：http://euw.hnxiangtu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uii.gogol.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ylz.nwbrower.top

JS:   await fetch(url)
来源：http://qca.fzhhl.top

TS:   await fetch(url)
来源：http://ton.snrcjt.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zqg.mhx1999.top

Go:   resp, err := http.Get(url)
来源：http://qwf.shangyingyoupin.top

Ruby: Net::HTTP.get(URI(url))
来源：http://xtq.ywan-chungtsiang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zxh.svipenyu.cn

[L02] 发送 POST JSON
来源：http://xrt.shangyingyoupin.top

Py:   requests.post(url, json={"a": 1})
来源：http://nqm.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uox.jiagoushi.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jyh.jyoumei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kgn.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bhp.hongshengwenyu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://isw.quarkkingdee.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zuq.yanxiufei.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tbd.hysaishi.cn

[L03] 设置自定义请求头
来源：http://bbm.smart0.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vzg.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://giy.andypj.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gbp.xziqi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jhg.zhixingplan.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mna.yj202588.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tka.fktsv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vjj.sxryk.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dgw.zhoulong.xyz

[L04] 设置超时
来源：http://khg.chenjidiqi.icu

Py:   requests.get(url, timeout=5)
来源：http://rod.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sss.ivvv.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://npr.wangdashe.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://goy.zdbjq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vhr.zhaomingkeji.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qvd.gotoacloud.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mav.wangdashe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://egb.pengpengdd.cyou

[L05] 上传文件（multipart）
来源：http://kom.shangyingyoupin.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kzo.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tdo.xylfe.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pau.andypj.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mff.yangfankeji.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://btx.yueranfly.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jvq.aizwys.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tvb.ywan-chungtsiang.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gfx.hfpthk.cn

[L06] 解析响应为 JSON
来源：http://cik.zdqjudy.top

Py:   resp.json()
来源：http://roj.aibaodan.cn

PHP:  json_decode($body, true);
来源：http://efy.sufxvd.cn

JS:   await resp.json()
来源：http://wnm.fengsongda.top

TS:   await resp.json()
来源：http://nqa.ehwqpu.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gss.jianghu66.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wtv.quarkkingdee.top

Ruby: JSON.parse(resp.body)
来源：http://ytc.daria6918.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ucb.gotoacloud.top


<!-- 参考信息 -->