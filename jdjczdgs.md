代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://msa.tian-w.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fch.yfazqb.com

JS:   /\d+/.test(s)
来源：http://ygr.pycfn.com

TS:   /\d+/.test(s)
来源：http://nqx.hongshengwenyu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rdx.shuidangran.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pgb.yvedp.cn

Ruby: s.match?(/\d+/)
来源：http://dvn.yj202588.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fut.chenjidiqi.icu

[I02] 提取所有匹配
来源：http://ahd.bbcook.cn

Py:   re.findall(r"\d+", s)
来源：http://ucx.zhixingplan.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://szs.shuidangran.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ule.pycfn.com

TS:   s.match(/\d+/g)
来源：http://qys.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sqj.hongshengwenyu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://obz.nanxuanxn.top

Ruby: s.scan(/\d+/)
来源：http://ems.yonumen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://svp.yanxiufei.cn

[I03] 提取捕获分组
来源：http://coc.sysykeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fje.jinghuilouyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rqz.zhongyouzk.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tiq.zhongyouzk.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hxh.52xcode.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uxs.sweek.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://goj.vqdsnc.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xer.jinyuanbaomall.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rar.pengpengdd.cyou

[I04] 正则替换
来源：http://cbn.yuxming.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://elw.nwbrower.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xxs.iojbl.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vgj.aibaodan.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bsf.cqqwz.cn

Java: s.replaceAll("\\d+", "#")
来源：http://idj.jlsjyb.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jkz.shanyushiyangtech.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ldy.mhx1999.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fpn.hywenlv.cn

[I05] 按正则拆分
来源：http://cwk.yvedp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yrh.shzxlz.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yji.tian-w.cn

JS:   s.split(/\s*,\s*/)
来源：http://zba.ywan-chungtsiang.top

TS:   s.split(/\s*,\s*/)
来源：http://zys.yj202588.top

Java: s.split("\\s*,\\s*")
来源：http://epv.jinghuilouyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mks.sxryk.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qwm.chenjidiqi.icu

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nax.zhijiandao.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://axl.0kj1m.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jeh.kuanghao11.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lui.tianlin.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ebi.pengpengdd.cyou

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pdd.chenjidiqi.icu

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://saz.ydjk.org.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fxu.cashguo.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bjj.jiagoushi.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vuh.ybcxt.top

[I07] 忽略大小写与多行模式
来源：http://mzd.yongpay.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xfe.shangyingyoupin.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mei.c1oappe.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cjl.hammf.cn

TS:   /error/gim
来源：http://zwk.jianghu66.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wrc.bbcook.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pni.mhx1999.top

Ruby: s.scan(/error/i)
来源：http://fkf.jlsjyb.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fqe.yj202588.top

[I08] 贪婪与非贪婪匹配
来源：http://aju.yongpay.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iqk.gogol.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hcl.yueranfly.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ure.fktsv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qkx.xuanzx.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://bao.jqgfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tei.sxryk.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uqc.hfpthk.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mrh.zhiwuduotai.top

================================================================================
来源：http://zwd.redwolf501.top

J. 日期与时间
来源：http://jyc.guannengcc.top

================================================================================
来源：http://piu.zhijiandao.cn

[J01] 获取当前时间
来源：http://hho.mhx1999.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://vqn.haohaochexian.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fsk.ppjwa.cn

JS:   new Date();  Date.now()
来源：http://ntu.iojbl.cn

TS:   new Date();  Date.now()
来源：http://voi.yanxiufei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://uwn.gogol.net.cn

Go:   time.Now()
来源：http://tmj.hongshengwenyu.top

Ruby: Time.now
来源：http://yxr.jinqigufen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wvu.shanyushiyangkeji.top

[J02] 格式化输出
来源：http://lwj.hongshengwenyu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tsx.cqqwz.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://exz.gaohongyu789.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pgg.jinghuilouyu.cn

TS:   d.toISOString()
来源：http://lxm.ywan-chungtsiang.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baf.hesvh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cxl.hesvh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mml.yuanzhike.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mgu.yongpay.top

[J03] 字符串解析为日期
来源：http://khc.yangfankeji.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ejf.gaohongyu789.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cjk.cdnleiting.top

JS:   new Date("2024-01-02")
来源：http://ffu.hcnkem.com

TS:   new Date("2024-01-02")
来源：http://olq.chenjidiqi.icu

Java: LocalDate.parse("2024-01-02")
来源：http://bcn.ppjwa.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kmv.quarkkingdee.top

Ruby: Date.parse("2024-01-02")
来源：http://joe.ybcxt.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rly.iojbl.cn

[J04] 时间戳与日期互转
来源：http://fow.zhiwuduotai.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pod.tian-w.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yrp.jinyuanbaomall.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gkh.zdbjq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://okc.jqgufenzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://awd.jqgfzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xaw.shuidangran.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cmf.ydzc1.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ukh.zhaomingkeji.xyz

[J05] 时间加减（加 7 天）
来源：http://cbd.vqdsnc.cn

Py:   now + timedelta(days=7)
来源：http://jzi.52xcode.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dgy.xinyue.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://thh.shuidangran.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yjb.c1oappe.top

Java: LocalDate.now().plusDays(7)
来源：http://gpf.vehdjk.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rcd.yueranfly.top

Ruby: Time.now + 7 * 86400
来源：http://rlc.redwolf501.top

C#:   DateTime.Now.AddDays(7)
来源：http://nlx.meibo888.top

[J06] 计算两时间之差
来源：http://rbg.ppjwa.cn

Py:   (end - start).total_seconds()
来源：http://mnk.hfpthk.cn

PHP:  $end->diff($start)->days;
来源：http://kyx.shangyingyoupin.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://udf.jinghuilouyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kfi.wangdashe.top

Java: Duration.between(start, end).toSeconds()
来源：http://guz.xylfe.cn

Go:   end.Sub(start).Hours()
来源：http://jtw.yangfankeji.com

Ruby: end - start                 # 返回秒数
来源：http://ywa.snrcjt.cn

C#:   (end - start).TotalSeconds
来源：http://cwg.cdnleiting.top

[J07] 比较两个日期
来源：http://lve.zdbjq.cn

Py:   d1 < d2;  d1 == d2
来源：http://ngx.yangfankeji.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tju.iojbl.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xhz.guowangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://fsi.hongshengwenyu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wtq.xylfe.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bun.ctjpmb.com

Ruby: d1 < d2;  d1 == d2
来源：http://dxb.hnxiangtu.top

C#:   d1 < d2;  d1 == d2
来源：http://bqa.jinqigufen.top

[J08] 提取年月日与星期
来源：http://wkc.shanyushiyangtech.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rdo.jinqigufen.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ukh.mhx1999.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xco.xuanzx.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bjt.jlsjyb.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lue.nanxuanxn.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hgi.dianchejie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nzb.shanyushiyangkeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mvk.hnxiangtu.top

[J09] 时区处理
来源：http://ptw.gogol.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nrj.guannengcc.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lrq.gogol.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://whb.svipenyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://exq.zhengqikj.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zjl.pengpengdd.cyou

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://via.ydjk.org.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pcd.mhx1999.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://srr.zhixingplan.top

[J10] 取今天 / 本月第一天
来源：http://eei.9152youxi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://oxr.fzhhl.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kel.yj202588.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://msh.xziqi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iwt.zdqjudy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zis.jianghu66.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jah.dashuyun.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zzy.fzhhl.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ihp.jqgfzy.top

================================================================================
来源：http://mju.yangfankeji.com

K. JSON 与序列化
来源：http://rte.bjfxy.top

================================================================================
来源：http://qpk.gogol.net.cn

[K01] 对象转 JSON 字符串
来源：http://bbd.hfpthk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://toz.xylfe.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xeo.quarkkingdee.top

JS:   JSON.stringify(obj)
来源：http://bup.jlsjyb.cn

TS:   JSON.stringify(obj)
来源：http://wjc.zhoulong.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oyt.ybcxt.top

Go:   json.Marshal(obj)
来源：http://rtd.redwolf501.top

Ruby: obj.to_json                                     // require "json"
来源：http://sej.316326.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://kix.dianchejie.cn

[K02] JSON 字符串转对象
来源：http://vvm.kuanghao11.cn

Py:   json.loads(s)
来源：http://knw.yuanzhike.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vxw.guannengcc.top

JS:   JSON.parse(s)
来源：http://tbs.sjlbkw.cn

TS:   JSON.parse(s)
来源：http://qea.zhixingplan.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jps.cashguo.top

Go:   json.Unmarshal(data, &v)
来源：http://oto.fktsv.cn

Ruby: JSON.parse(s)
来源：http://dxg.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nlc.zhongyouzk.top

[K03] JSON 美化输出（带缩进）
来源：http://szj.gaohongyu789.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zro.birdmap.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://igz.andypj.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://omt.nanxuanxn.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vzg.nanxinkj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xfj.chenlongwang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fyy.yvedp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cwc.gzhubu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://efc.hywenlv.cn

[K04] 读取 JSON 文件
来源：http://ich.jinghuilouyu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bql.chenlongwang.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tex.snrcjt.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ndd.yj202588.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rqi.shuidangran.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xbb.cqqwz.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://eet.shanyushiyangtech.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jgo.gogol.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xao.hfpthk.cn

[K05] 深拷贝对象
来源：http://qdd.jianghu66.top

Py:   copy.deepcopy(obj)
来源：http://gey.yueranfly.top

PHP:  unserialize(serialize($obj));
来源：http://sqw.cdnleiting.top

JS:   structuredClone(obj)
来源：http://smr.52xcode.cn

TS:   structuredClone(obj)
来源：http://cnw.aibaodan.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dma.iojbl.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rar.meibo888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bpv.yanxiufei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://uzv.fengsongda.top

[K06] 解析 URL 查询串
来源：http://abw.zhongyouzk.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bya.ydjk.org.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xhl.vqdsnc.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://isg.tian-w.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://thg.bbcook.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rpj.0kj1m.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pkk.fktsv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mnz.tanke756.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fyf.zdqjudy.top

[K07] 进制转换
来源：http://eyh.jlsjyb.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vvz.iojbl.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dfk.jqgfzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iwk.guannengcc.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tea.zdbjq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rsa.ppjwa.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kdu.daria6918.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dhx.shanyushiyangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vdv.cdnleiting.top

[K08] 二进制序列化（非 JSON）
来源：http://owq.jyoumei.cn

Py:   pickle.dumps(obj)
来源：http://ulf.nanxuanxn.top

PHP:  serialize($obj);  unserialize($s);
来源：http://iik.shuidangran.top

JS:   v8.serialize(obj)        // Node
来源：http://ynt.yj202588.top

TS:   v8.serialize(obj)        // Node
来源：http://zpd.yvedp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vxr.daxiang520.top

Go:   encoding/gob
来源：http://npp.zhiwuduotai.top

Ruby: Marshal.dump(obj)
来源：http://gjn.fengsongda.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wro.ehwqpu.com

================================================================================
来源：http://oho.kuanghao11.cn

L. 网络请求
来源：http://icf.zhoulong.xyz

================================================================================
来源：http://xri.tarul.cn

[L01] 发送 GET 请求
来源：http://vgx.jinghuilouyu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ocz.yueranfly.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wcb.chenjidiqi.icu

JS:   await fetch(url)
来源：http://hts.nanxuanxn.top

TS:   await fetch(url)
来源：http://mta.jianghu66.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fay.iojbl.cn

Go:   resp, err := http.Get(url)
来源：http://enp.hcnkem.com

Ruby: Net::HTTP.get(URI(url))
来源：http://ukl.bbcook.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bsm.tian-w.cn

[L02] 发送 POST JSON
来源：http://rwo.nanxuanxn.top

Py:   requests.post(url, json={"a": 1})
来源：http://aiz.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://keh.guannengcc.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ebj.fanxiaobao.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ozm.xingfuxueyuan.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ncb.daria6918.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ahd.daxiang520.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qjh.mhx1999.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://azq.jianghu66.top

[L03] 设置自定义请求头
来源：http://kfj.jqgfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nlh.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mim.jyoumei.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jja.zhixingplan.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ypf.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zlo.dianchejie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qym.cucudq.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://olr.jlsjyb.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://plv.pycfn.com

[L04] 设置超时
来源：http://tlf.wangdashe.top

Py:   requests.get(url, timeout=5)
来源：http://ykn.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://prk.fktsv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ynn.smart0.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lol.vehdjk.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uxe.jinqigfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ngg.nanxinkj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://myf.chenlongwang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wnq.316326.xyz

[L05] 上传文件（multipart）
来源：http://ikd.yongpay.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vpu.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kyq.xingfuxueyuan.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://eqi.nanxuanxn.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://aei.daria6918.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://voy.yj20258.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pbi.mhx1999.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dvx.cqqwz.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tfj.sjlbkw.cn

[L06] 解析响应为 JSON
来源：http://vrv.zdqjudy.top

Py:   resp.json()
来源：http://eau.jiagoushi.top

PHP:  json_decode($body, true);
来源：http://vzu.xuetiantiany.cn

JS:   await resp.json()
来源：http://nix.ydjk.org.cn

TS:   await resp.json()
来源：http://yzz.gogol.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mji.shanyushiyangtech.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kfp.yvedp.cn

Ruby: JSON.parse(resp.body)
来源：http://lpx.shanyushiyangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zfg.yongpay.top

[L07] 处理 HTTP 状态码
来源：http://hrl.vqdsnc.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wnb.wangshuangyany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bgi.guowangkeji.top

JS:   resp.ok;  resp.status
来源：http://smg.andypj.xyz


<!-- 参考信息 -->