代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pnv.tarul.cn

Go:   defer f.Close()
来源：http://qrn.epnwcf.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jop.chenzaomai.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bja.316326.xyz

================================================================================
来源：http://www.yangfankeji.com

I. 正则表达式
来源：http://lqt.guowangkeji.top

================================================================================
来源：http://yzc.9152youxi.cn

[I01] 判断是否匹配
来源：http://maq.sysykeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wwh.hfpthk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://odx.ywan-chungtsiang.top

JS:   /\d+/.test(s)
来源：http://ful.0kj1m.cn

TS:   /\d+/.test(s)
来源：http://buq.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://diz.quarkkingdee.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hfd.svipenyu.cn

Ruby: s.match?(/\d+/)
来源：http://pdm.hnxiangtu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://eko.hysaishi.cn

[I02] 提取所有匹配
来源：http://ecm.guannengcc.top

Py:   re.findall(r"\d+", s)
来源：http://dxz.svipenyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zpu.hywenlv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://agb.sufxvd.cn

TS:   s.match(/\d+/g)
来源：http://ddo.sweek.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://utq.pengpengdd.cyou

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tif.bjfxy.top

Ruby: s.scan(/\d+/)
来源：http://qya.gaohongyu789.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vfn.jiagoushi.top

[I03] 提取捕获分组
来源：http://gcf.nanxinkj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pah.hnqzz.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tot.daria6918.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dze.pycfn.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pzy.ehwqpu.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hrn.jlsjyb.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vni.guowangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cvv.cqqwz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lzx.cucudq.cn

[I04] 正则替换
来源：http://rps.xuanzx.com

Py:   re.sub(r"\d+", "#", s)
来源：http://ziv.shzxlz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://shm.wangshuangyany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pqe.hywenlv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ksx.ctjpmb.com

Java: s.replaceAll("\\d+", "#")
来源：http://ret.dashuyun.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nng.shzxlz.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lhd.gzhubu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nrk.zhixingplan.top

[I05] 按正则拆分
来源：http://efr.jinyuanbaomall.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cuu.shanyushiyangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ijl.gogol.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://gpi.yangfankeji.com

TS:   s.split(/\s*,\s*/)
来源：http://gkf.ctjpmb.com

Java: s.split("\\s*,\\s*")
来源：http://cfb.kuanghao11.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zyy.vehdjk.com

Ruby: s.split(/\s*,\s*/)
来源：http://iji.wangdashe.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gmq.ctjpmb.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cas.hysaishi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qeh.tian-w.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://viy.xuanzx.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://etr.yanxiufei.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vem.yangfankeji.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://smb.nanxinkj.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xsa.daria6918.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://raf.nanxuanxn.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nti.jinghuilouyu.cn

[I07] 忽略大小写与多行模式
来源：http://gnk.fktsv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tjp.chenlongwang.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bja.xziqi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mhq.uphjek.com

TS:   /error/gim
来源：http://mem.yuanzhike.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xoo.9152youxi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fuv.andypj.xyz

Ruby: s.scan(/error/i)
来源：http://ihq.yj20258.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bpn.tarul.cn

[I08] 贪婪与非贪婪匹配
来源：http://mjl.sxryk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ybz.zhijiandao.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uxv.hammf.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kfi.mhx1999.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dsf.yuxming.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tuw.guowangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kqf.ehwqpu.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rbx.shuidangran.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mau.vehdjk.com

================================================================================
来源：http://pyq.ehwqpu.com

J. 日期与时间
来源：http://yvm.kuanghao11.cn

================================================================================
来源：http://azo.hysaishi.cn

[J01] 获取当前时间
来源：http://okx.shuidangran.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://rja.yj20258.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vlq.nanxuanxn.top

JS:   new Date();  Date.now()
来源：http://liy.tian-w.cn

TS:   new Date();  Date.now()
来源：http://deb.pycfn.com

Java: LocalDateTime.now();  Instant.now()
来源：http://hbz.redwolf501.top

Go:   time.Now()
来源：http://rit.quarkkingdee.top

Ruby: Time.now
来源：http://pep.yueranfly.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uwc.yongpay.top

[J02] 格式化输出
来源：http://ntj.yfazqb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xew.zhiwuduotai.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rjf.hfpthk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dcq.dianchejie.cn

TS:   d.toISOString()
来源：http://msp.9152youxi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://agw.sufxvd.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://feg.kuanghao11.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://him.sysykeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://eoo.shzxlz.cn

[J03] 字符串解析为日期
来源：http://vxt.vqdsnc.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zod.shuidangran.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vva.zhiwuduotai.top

JS:   new Date("2024-01-02")
来源：http://jpn.epnwcf.com

TS:   new Date("2024-01-02")
来源：http://ksj.yuanzhike.top

Java: LocalDate.parse("2024-01-02")
来源：http://tuc.hysaishi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oxo.meibo888.top

Ruby: Date.parse("2024-01-02")
来源：http://gov.fanxiaobao.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://iab.cqqwz.cn

[J04] 时间戳与日期互转
来源：http://pdh.9152youxi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://whi.fanxiaobao.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ajj.xuanzx.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mbz.c1oappe.top

TS:   Math.floor(Date.now() / 1000)
来源：http://pjp.shzxlz.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mqk.andypj.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ffx.pengpengdd.cyou

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cfm.vehdjk.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cgr.tian-w.cn

[J05] 时间加减（加 7 天）
来源：http://mip.yvedp.cn

Py:   now + timedelta(days=7)
来源：http://cht.shuidangran.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pis.aibaodan.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lzs.xingfuxueyuan.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tho.sysykeji.top

Java: LocalDate.now().plusDays(7)
来源：http://bhs.jinqigfzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ufa.hammf.cn

Ruby: Time.now + 7 * 86400
来源：http://dml.hysaishi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jxs.wangdashe.top

[J06] 计算两时间之差
来源：http://sbk.ehwqpu.com

Py:   (end - start).total_seconds()
来源：http://zvv.gogol.net.cn

PHP:  $end->diff($start)->days;
来源：http://tjf.ydjk.org.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pow.cheryme.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dsx.cucudq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://izl.ehwqpu.com

Go:   end.Sub(start).Hours()
来源：http://lwr.shanyushiyangtech.top

Ruby: end - start                 # 返回秒数
来源：http://bxy.zhixingplan.top

C#:   (end - start).TotalSeconds
来源：http://zas.bjfxy.top

[J07] 比较两个日期
来源：http://pqr.tian-w.cn

Py:   d1 < d2;  d1 == d2
来源：http://ccy.nanxinkj.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://anb.kuanghao11.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zls.mhx1999.top

TS:   d1.getTime() < d2.getTime()
来源：http://ohv.sufxvd.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wmx.jqgfzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qdn.hysaishi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sgu.jinyuanbaomall.cn

C#:   d1 < d2;  d1 == d2
来源：http://atc.iojbl.cn

[J08] 提取年月日与星期
来源：http://gdt.xinyue.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ocb.mhx1999.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xoq.mhx1999.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lla.zdbjq.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lfz.sjlbkw.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bec.yfazqb.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mel.c1oappe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rsh.birdmap.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ial.xuetiantiany.cn

[J09] 时区处理
来源：http://pyv.chenjidiqi.icu

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qlg.fehbvm.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pyv.yongpay.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nuu.zdbjq.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dcb.quarkkingdee.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dqu.zhongyouzk.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://htw.gzhubu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ykb.aibaodan.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iqv.pengpengdd.cyou

[J10] 取今天 / 本月第一天
来源：http://rji.redwolf501.top

Py:   date.today();  date.today().replace(day=1)
来源：http://pfn.chenjidiqi.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vsl.0kj1m.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rxa.uphjek.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://aro.sxryk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rox.yfazqb.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jfg.yangfankeji.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vtw.jqgfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ecp.jinqigufen.top

================================================================================
来源：http://yyb.cucudq.cn

K. JSON 与序列化
来源：http://grr.zhiwuduotai.top

================================================================================
来源：http://dvw.sxryk.cn

[K01] 对象转 JSON 字符串
来源：http://ykn.yfazqb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fah.tian-w.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yhs.dianchejie.cn

JS:   JSON.stringify(obj)
来源：http://ibi.jinqigufen.top

TS:   JSON.stringify(obj)
来源：http://qod.nanxuanxn.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ret.havefunace.top

Go:   json.Marshal(obj)
来源：http://ips.zdbjq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uzn.shanyushiyangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://lcl.zhixingplan.top

[K02] JSON 字符串转对象
来源：http://bvd.havefunace.top

Py:   json.loads(s)
来源：http://afk.hfpthk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iwf.cucudq.cn

JS:   JSON.parse(s)
来源：http://ree.jqgfzy.top

TS:   JSON.parse(s)
来源：http://vzq.ybcxt.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wds.andypj.xyz

Go:   json.Unmarshal(data, &v)
来源：http://dil.jlsjyb.cn

Ruby: JSON.parse(s)
来源：http://nwq.bjfxy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blj.yueranfly.top

[K03] JSON 美化输出（带缩进）
来源：http://uyj.cucudq.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qzb.vqdsnc.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://crx.andypj.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://hfq.bjfxy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://zdo.sweek.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eft.gaohongyu789.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vwx.9152youxi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://enq.yuxming.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tvz.daria6918.cn

[K04] 读取 JSON 文件
来源：http://plt.mhx1999.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wlv.hnqzz.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://unk.yuanzhike.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jtd.nanxuanxn.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zwk.yj20258.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kkv.ehwqpu.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hdb.daxiang520.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ifg.fehbvm.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pou.sysykeji.top

[K05] 深拷贝对象
来源：http://teg.zhoulong.xyz

Py:   copy.deepcopy(obj)
来源：http://obm.epnwcf.com

PHP:  unserialize(serialize($obj));
来源：http://vkp.cucudq.cn

JS:   structuredClone(obj)
来源：http://oln.nanxinkj.top

TS:   structuredClone(obj)
来源：http://hev.xinyue.icu

Java: // 手写拷贝构造，或序列化往返
来源：http://tgh.zhijiandao.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vmk.guowangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lnz.fanxiaobao.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://dqf.daxiang520.top

[K06] 解析 URL 查询串
来源：http://mzm.tarul.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tsi.316326.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ras.xziqi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hlm.cucudq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pgw.hesvh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uvp.hcnkem.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://oqr.pengpengdd.cyou

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gur.andypj.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ujx.tarul.cn

[K07] 进制转换
来源：http://ipc.cucudq.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fwr.daxiang520.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uxn.tarul.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yeg.hongshengwenyu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vrv.havefunace.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fry.fktsv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kru.pengpengdd.cyou

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eeb.zhoulong.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zul.yuxming.cn

[K08] 二进制序列化（非 JSON）
来源：http://xrp.tarul.cn

Py:   pickle.dumps(obj)
来源：http://daj.pengpengdd.cyou

PHP:  serialize($obj);  unserialize($s);
来源：http://kba.9152youxi.cn

JS:   v8.serialize(obj)        // Node
来源：http://eug.tianlin.xyz

TS:   v8.serialize(obj)        // Node
来源：http://jyb.0kj1m.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kgz.jyoumei.cn

Go:   encoding/gob
来源：http://tak.quarkkingdee.top

Ruby: Marshal.dump(obj)
来源：http://dov.svipenyu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gag.guannengcc.top

================================================================================
来源：http://alh.shzxlz.cn

L. 网络请求
来源：http://sjh.gogol.net.cn

================================================================================
来源：http://jbq.gzhubu.top

[L01] 发送 GET 请求
来源：http://une.nanxinkj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ruu.yanxiufei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://acm.cdnleiting.top

JS:   await fetch(url)
来源：http://gth.fengsongda.top

TS:   await fetch(url)
来源：http://jrf.havefunace.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pat.jianghu66.top

Go:   resp, err := http.Get(url)
来源：http://ywo.uphjek.com

Ruby: Net::HTTP.get(URI(url))
来源：http://xmf.cheryme.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xco.ivvv.top

[L02] 发送 POST JSON
来源：http://wgp.cucudq.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tcs.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wxy.zycfv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iyt.yj202588.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ugy.hfpthk.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jhj.tanke756.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xyt.bjfxy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cjz.dianchejie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zkf.shanyushiyangtech.top

[L03] 设置自定义请求头
来源：http://saw.pengpengdd.cyou

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hgc.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://eqp.hnxiangtu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mat.wangdashe.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aez.gogol.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ykv.shuidangran.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vfw.epnwcf.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kqk.yueranfly.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ugp.gzhubu.top

[L04] 设置超时
来源：http://mdl.shzxlz.cn

Py:   requests.get(url, timeout=5)
来源：http://gju.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bpb.tanke756.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jrr.yj202588.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zem.hfpthk.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gqs.zdqjudy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sbc.yueranfly.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qco.yanxiufei.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hjz.ivvv.top

[L05] 上传文件（multipart）
来源：http://rsv.hywenlv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mnl.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qba.cucudq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wpm.chenzaomai.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://snw.guannengcc.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wkj.c1oappe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cqu.shanyushiyangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iny.vehdjk.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://srq.c1oappe.top

[L06] 解析响应为 JSON
来源：http://qta.shanyushiyangkeji.top

Py:   resp.json()
来源：http://wlw.dianchejie.cn

PHP:  json_decode($body, true);
来源：http://crc.shangyingyoupin.top

JS:   await resp.json()
来源：http://lys.dianchejie.cn

TS:   await resp.json()
来源：http://jxo.cucudq.cn


<!-- 参考信息 -->