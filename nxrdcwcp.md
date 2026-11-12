代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://iav.snrcjt.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fri.bjfxy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wqs.guannengcc.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wgx.gaohongyu789.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gft.zdbjq.cn

Go:   defer f.Close()
来源：http://giw.fengsongda.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jcv.zhoulong.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://opn.xingfuxueyuan.xyz

================================================================================
来源：http://iqh.tianlin.xyz

I. 正则表达式
来源：http://fgi.mhx1999.top

================================================================================
来源：http://qlj.cheryme.top

[I01] 判断是否匹配
来源：http://ibq.cqqwz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sdo.jinqigfzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://vnz.mhx1999.top

JS:   /\d+/.test(s)
来源：http://qvx.ppjwa.cn

TS:   /\d+/.test(s)
来源：http://wjv.yueranfly.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nfk.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mwn.ehwqpu.com

Ruby: s.match?(/\d+/)
来源：http://gun.nanxuanxn.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://miw.jyoumei.cn

[I02] 提取所有匹配
来源：http://ptj.fzhhl.top

Py:   re.findall(r"\d+", s)
来源：http://lzo.ivvv.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xaj.guannengcc.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://olo.iojbl.cn

TS:   s.match(/\d+/g)
来源：http://ldn.smart0.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://iiw.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://htm.guowangkeji.top

Ruby: s.scan(/\d+/)
来源：http://szr.hfpthk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://urm.hywenlv.cn

[I03] 提取捕获分组
来源：http://xgo.jianghu66.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://god.daria6918.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mat.yanxiufei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mmj.fehbvm.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dkd.hongshengwenyu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rci.hnxiangtu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yxm.cheryme.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gcp.9152youxi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dzt.ctjpmb.com

[I04] 正则替换
来源：http://lyl.c1oappe.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mmg.tarul.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wfa.daxiang520.top

JS:   s.replace(/\d+/g, "#")
来源：http://tzc.chenlongwang.top

TS:   s.replace(/\d+/g, "#")
来源：http://pfz.gaohongyu789.top

Java: s.replaceAll("\\d+", "#")
来源：http://gxf.zdqjudy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://mwp.zhijiandao.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lxs.cqqwz.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kkc.feifeiyinyue.top

[I05] 按正则拆分
来源：http://uwy.iojbl.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://szo.zdqjudy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mwn.jqgfzy.top

JS:   s.split(/\s*,\s*/)
来源：http://lqa.chenjidiqi.icu

TS:   s.split(/\s*,\s*/)
来源：http://aji.ybcxt.top

Java: s.split("\\s*,\\s*")
来源：http://guu.hnxiangtu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gxd.jinyuanbaomall.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nph.yvedp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ihe.dianchejie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xvf.xuetiantiany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eeo.yj202588.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rvm.yangfankeji.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ukq.fanxiaobao.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hhp.ppjwa.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kkx.vehdjk.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vza.yj20258888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qrc.zycfv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gon.yonumen.top

[I07] 忽略大小写与多行模式
来源：http://fuo.hesvh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ikw.zhongyouzk.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mon.sweek.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hlc.jiagoushi.top

TS:   /error/gim
来源：http://lus.meibo888.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ydb.sjlbkw.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cmc.wangshuangyany.cn

Ruby: s.scan(/error/i)
来源：http://tsq.yfazqb.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vog.yvedp.cn

[I08] 贪婪与非贪婪匹配
来源：http://ndh.zhongyouzk.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://udc.gogol.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dcl.sxryk.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qnt.yonumen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qbx.zhijiandao.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xfn.chenzaomai.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ysj.chenzaomai.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vpu.zhiwuduotai.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://abq.yangfankeji.com

================================================================================
来源：http://hnw.shangyingyoupin.top

J. 日期与时间
来源：http://jdh.shuidangran.top

================================================================================
来源：http://enn.zdbjq.cn

[J01] 获取当前时间
来源：http://jmc.zhaomingkeji.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://oac.wangshuangyany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lhq.hnqzz.top

JS:   new Date();  Date.now()
来源：http://kzy.ydjk.org.cn

TS:   new Date();  Date.now()
来源：http://fxt.fehbvm.com

Java: LocalDateTime.now();  Instant.now()
来源：http://wlg.hcnkem.com

Go:   time.Now()
来源：http://fvb.havefunace.top

Ruby: Time.now
来源：http://wbm.bbcook.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jub.yonumen.top

[J02] 格式化输出
来源：http://typ.shzxlz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pcq.jyoumei.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tcj.yanxiufei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://egz.zycfv.cn

TS:   d.toISOString()
来源：http://drq.shzxlz.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nhi.yangfankeji.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kjz.shangyingyoupin.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ytw.xingfuxueyuan.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://irk.shzxlz.cn

[J03] 字符串解析为日期
来源：http://plt.daxiang520.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lrz.yueranfly.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xuq.sjlbkw.cn

JS:   new Date("2024-01-02")
来源：http://rle.c1oappe.top

TS:   new Date("2024-01-02")
来源：http://pzk.vqdsnc.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vcn.shanyushiyangkeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://apc.sjlbkw.cn

Ruby: Date.parse("2024-01-02")
来源：http://mbs.chenlongwang.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cdi.gaohongyu789.top

[J04] 时间戳与日期互转
来源：http://lrp.yj202588.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dgs.bjfxy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://viq.jinqigufen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://snd.smart0.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://tix.fengsongda.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eum.chenlongwang.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://srv.yj202588.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mvs.snrcjt.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://osn.zhoulong.xyz

[J05] 时间加减（加 7 天）
来源：http://hcn.tarul.cn

Py:   now + timedelta(days=7)
来源：http://kkb.yangfankeji.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://qja.zhongyouzk.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qbe.fehbvm.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://psu.aibaodan.cn

Java: LocalDate.now().plusDays(7)
来源：http://roi.jqgfzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ckt.wangshuangyany.cn

Ruby: Time.now + 7 * 86400
来源：http://jxg.fehbvm.com

C#:   DateTime.Now.AddDays(7)
来源：http://qaw.yangfankeji.com

[J06] 计算两时间之差
来源：http://tpb.nanxuanxn.top

Py:   (end - start).total_seconds()
来源：http://kej.chenjidiqi.icu

PHP:  $end->diff($start)->days;
来源：http://ape.fzhhl.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jjj.sysykeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://usu.zdbjq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://htr.shangyingyoupin.top

Go:   end.Sub(start).Hours()
来源：http://hbq.ppjwa.cn

Ruby: end - start                 # 返回秒数
来源：http://rja.0kj1m.cn

C#:   (end - start).TotalSeconds
来源：http://yam.smart0.xyz

[J07] 比较两个日期
来源：http://who.hammf.cn

Py:   d1 < d2;  d1 == d2
来源：http://jfp.jyoumei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wvk.bjfxy.top

JS:   d1.getTime() < d2.getTime()
来源：http://flw.birdmap.top

TS:   d1.getTime() < d2.getTime()
来源：http://pvn.hammf.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oox.yonumen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mdv.jqgufenzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://hya.daria6918.cn

C#:   d1 < d2;  d1 == d2
来源：http://fvg.aibaodan.cn

[J08] 提取年月日与星期
来源：http://dlx.ywan-chungtsiang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nsl.guowangkeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lvc.yj202588.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://izn.ivvv.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qot.vehdjk.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gap.birdmap.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tla.chenlongwang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://irw.hcnkem.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fnq.cashguo.top

[J09] 时区处理
来源：http://izq.yvedp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wtz.zhengqikj.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://huh.zhijiandao.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zxg.chenjidiqi.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://khp.52xcode.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://usm.pycfn.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vfl.ivvv.top

Ruby: Time.now.getlocal("+08:00")
来源：http://cec.fzhhl.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jpy.cucudq.cn

[J10] 取今天 / 本月第一天
来源：http://tzn.vehdjk.com

Py:   date.today();  date.today().replace(day=1)
来源：http://wst.hysaishi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kfi.jlsjyb.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pvp.cucudq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vyx.gogol.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rbb.zycfv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ves.quarkkingdee.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cfz.havefunace.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tax.ydjk.org.cn

================================================================================
来源：http://yui.jianghu66.top

K. JSON 与序列化
来源：http://drc.epnwcf.com

================================================================================
来源：http://fto.tanke756.top

[K01] 对象转 JSON 字符串
来源：http://gok.jiagoushi.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rrx.jinghuilouyu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xat.tianlin.xyz

JS:   JSON.stringify(obj)
来源：http://kkr.ybcxt.top

TS:   JSON.stringify(obj)
来源：http://let.cdnleiting.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hhd.zhixingplan.top

Go:   json.Marshal(obj)
来源：http://eoe.hywenlv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wga.xziqi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ezg.aibaodan.cn

[K02] JSON 字符串转对象
来源：http://owe.cdnleiting.top

Py:   json.loads(s)
来源：http://kjt.xingfuxueyuan.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://esd.hongshengwenyu.top

JS:   JSON.parse(s)
来源：http://ufz.cucudq.cn

TS:   JSON.parse(s)
来源：http://nsy.guannengcc.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kwo.sweek.top

Go:   json.Unmarshal(data, &v)
来源：http://vqv.nanxinkj.top

Ruby: JSON.parse(s)
来源：http://qiw.havefunace.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://swb.yongpay.top

[K03] JSON 美化输出（带缩进）
来源：http://rxe.guowangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xig.yuxming.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lyy.c1oappe.top

JS:   JSON.stringify(obj, null, 2)
来源：http://omv.fanxiaobao.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://rop.zhengqikj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rkz.andypj.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bzx.52xcode.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ske.shzxlz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tlw.yuxming.cn

[K04] 读取 JSON 文件
来源：http://eji.ywan-chungtsiang.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mhl.xingfuxueyuan.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zos.fanxiaobao.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ics.meibo888.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://awc.shuidangran.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vyc.pycfn.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://smo.cucudq.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://khg.guannengcc.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rxs.havefunace.top

[K05] 深拷贝对象
来源：http://kbj.tarul.cn

Py:   copy.deepcopy(obj)
来源：http://mkn.hammf.cn

PHP:  unserialize(serialize($obj));
来源：http://kjb.epnwcf.com

JS:   structuredClone(obj)
来源：http://hft.snrcjt.cn

TS:   structuredClone(obj)
来源：http://mbv.guannengcc.top

Java: // 手写拷贝构造，或序列化往返
来源：http://zlh.chenzaomai.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gtw.guannengcc.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tab.jiagoushi.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ogd.iojbl.cn

[K06] 解析 URL 查询串
来源：http://rde.yangfankeji.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vxd.bjfxy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kfw.cashguo.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uko.vqdsnc.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ntr.wangshuangyany.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mho.jqgufenzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cbf.9152youxi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rzt.jinqigufen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lid.hesvh.cn

[K07] 进制转换
来源：http://xks.xingfuxueyuan.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uvr.ivvv.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qvg.jinyuanbaomall.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jea.ctjpmb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mix.zhongyouzk.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://psw.tanke756.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://scq.havefunace.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vmb.havefunace.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pdo.xinyue.icu

[K08] 二进制序列化（非 JSON）
来源：http://dkn.ctjpmb.com

Py:   pickle.dumps(obj)
来源：http://pba.sysykeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://boj.gogol.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://csu.yanxiufei.cn

TS:   v8.serialize(obj)        // Node
来源：http://tpf.cqqwz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ylh.ydjk.org.cn

Go:   encoding/gob
来源：http://cnr.zhengqikj.top

Ruby: Marshal.dump(obj)
来源：http://fjh.yj20258.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://umv.wangshuangyany.cn

================================================================================
来源：http://mwv.dianchejie.cn

L. 网络请求
来源：http://odw.sweek.top

================================================================================
来源：http://nxe.guannengcc.top

[L01] 发送 GET 请求
来源：http://hiw.hywenlv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lgz.tian-w.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tom.tarul.cn

JS:   await fetch(url)
来源：http://mya.ctjpmb.com

TS:   await fetch(url)
来源：http://gyt.tianlin.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bpu.tian-w.cn

Go:   resp, err := http.Get(url)
来源：http://moe.hysaishi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vwc.sweek.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rbb.sweek.top

[L02] 发送 POST JSON
来源：http://yef.epnwcf.com

Py:   requests.post(url, json={"a": 1})
来源：http://aik.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fsm.shanyushiyangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gql.iojbl.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qyk.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bcp.zhoulong.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://htf.hnxiangtu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fex.sysykeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ezt.epnwcf.com

[L03] 设置自定义请求头
来源：http://udg.guowangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dgd.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bvo.uphjek.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wpq.sweek.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mdk.cqqwz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zvf.vehdjk.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xny.daria6918.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dxu.tian-w.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vkd.aibaodan.cn

[L04] 设置超时
来源：http://fxi.0kj1m.cn

Py:   requests.get(url, timeout=5)
来源：http://fav.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ivz.tarul.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://elw.xingfuxueyuan.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gwi.wangdashe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://iar.gaohongyu789.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ngv.wangshuangyany.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vjl.yueranfly.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hfp.gotoacloud.top

[L05] 上传文件（multipart）
来源：http://cwi.hammf.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tih.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ilf.tanke756.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hjc.feifeiyinyue.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xkc.zhongyouzk.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ice.aibaodan.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://get.iojbl.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ttb.zhijiandao.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fbq.shanyushiyangkeji.top

[L06] 解析响应为 JSON
来源：http://toh.aibaodan.cn


<!-- 参考信息 -->