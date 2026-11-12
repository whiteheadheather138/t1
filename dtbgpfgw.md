代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kkq.hammf.cn

Ruby: raise MyError.new("fail", 500)
来源：http://txf.pengpengdd.cyou

C#:   // 自定义异常类中加 Code 属性
来源：http://vsq.xinyue.icu

[H10] 资源自动释放
来源：http://tpu.shuidangran.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lpt.iojbl.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://erw.sjlbkw.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mfm.gotoacloud.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lgd.fanxiaobao.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://czt.hnqzz.top

Go:   defer f.Close()
来源：http://swy.shzxlz.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://emo.tarul.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hxt.fktsv.cn

================================================================================
来源：http://odi.daria6918.cn

I. 正则表达式
来源：http://uyx.svipenyu.cn

================================================================================
来源：http://jlt.pengpengdd.cyou

[I01] 判断是否匹配
来源：http://ezd.jqgufenzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bdu.yanxiufei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gqr.jinghuilouyu.cn

JS:   /\d+/.test(s)
来源：http://vou.nwbrower.top

TS:   /\d+/.test(s)
来源：http://gic.yonumen.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mot.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://idi.zdbjq.cn

Ruby: s.match?(/\d+/)
来源：http://wwo.kuanghao11.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dro.vehdjk.com

[I02] 提取所有匹配
来源：http://ksa.fehbvm.com

Py:   re.findall(r"\d+", s)
来源：http://dgz.cashguo.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ffb.sufxvd.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ilf.zhixingplan.top

TS:   s.match(/\d+/g)
来源：http://szw.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://afw.uphjek.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ewr.dashuyun.cn

Ruby: s.scan(/\d+/)
来源：http://cym.ywan-chungtsiang.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lna.yvedp.cn

[I03] 提取捕获分组
来源：http://wdh.yuanzhike.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zuq.pycfn.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ioo.tarul.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ook.dashuyun.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mpy.chenzaomai.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://poy.xuanzx.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gfi.cucudq.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://amn.yonumen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ndy.gogol.net.cn

[I04] 正则替换
来源：http://irg.c1oappe.top

Py:   re.sub(r"\d+", "#", s)
来源：http://bvz.shangyingyoupin.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bxx.hysaishi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jxe.gaohongyu789.top

TS:   s.replace(/\d+/g, "#")
来源：http://qua.zhengqikj.top

Java: s.replaceAll("\\d+", "#")
来源：http://yjm.tarul.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://huy.9152youxi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://iln.dashuyun.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://edr.aizwys.cn

[I05] 按正则拆分
来源：http://vnu.zdbjq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hkr.pycfn.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vht.havefunace.top

JS:   s.split(/\s*,\s*/)
来源：http://vbj.ywan-chungtsiang.top

TS:   s.split(/\s*,\s*/)
来源：http://xda.zhijiandao.cn

Java: s.split("\\s*,\\s*")
来源：http://kta.jianghu66.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lyl.sysykeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://wkk.yonumen.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rdj.nanxuanxn.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://eio.gaohongyu789.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xvo.guannengcc.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dnk.ctjpmb.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ejg.aizwys.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bpm.iojbl.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qrg.yangfankeji.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dbz.cucudq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kgd.svipenyu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dum.9152youxi.cn

[I07] 忽略大小写与多行模式
来源：http://qkb.dianchejie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bfg.bbcook.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hkg.tarul.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rfq.zhoulong.xyz

TS:   /error/gim
来源：http://ujp.zhaomingkeji.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yjz.hfpthk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://far.yueranfly.top

Ruby: s.scan(/error/i)
来源：http://gdg.daxiang520.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vke.yj202588.top

[I08] 贪婪与非贪婪匹配
来源：http://nmw.hongshengwenyu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ifg.yonumen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mhh.dianchejie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ljs.ydjk.org.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bvc.zhijiandao.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://pfj.jinghuilouyu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kdo.ppjwa.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uyj.52xcode.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://efw.xuetiantiany.cn

================================================================================
来源：http://vam.zhiwuduotai.top

J. 日期与时间
来源：http://pff.zdbjq.cn

================================================================================
来源：http://syw.wangdashe.top

[J01] 获取当前时间
来源：http://soc.uphjek.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://xrw.zdbjq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bdc.xuetiantiany.cn

JS:   new Date();  Date.now()
来源：http://nwe.shanyushiyangtech.top

TS:   new Date();  Date.now()
来源：http://knc.tanke756.top

Java: LocalDateTime.now();  Instant.now()
来源：http://mcl.ybcxt.top

Go:   time.Now()
来源：http://iwz.cdnleiting.top

Ruby: Time.now
来源：http://bta.uphjek.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hab.aibaodan.cn

[J02] 格式化输出
来源：http://tvo.jinyuanbaomall.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xfv.daria6918.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tgf.hcnkem.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nzn.meibo888.top

TS:   d.toISOString()
来源：http://tet.mhx1999.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dnn.yvedp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zts.aibaodan.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iqh.xingfuxueyuan.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ide.gaohongyu789.top

[J03] 字符串解析为日期
来源：http://uwc.zhongyouzk.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kpp.zhongyouzk.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jvr.aizwys.cn

JS:   new Date("2024-01-02")
来源：http://mbv.fktsv.cn

TS:   new Date("2024-01-02")
来源：http://ewp.jqgfzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://oxu.hcnkem.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qtf.shanyushiyangtech.top

Ruby: Date.parse("2024-01-02")
来源：http://qic.gaohongyu789.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://umd.tianlin.xyz

[J04] 时间戳与日期互转
来源：http://hod.cdnleiting.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fif.kuanghao11.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zud.zhongyouzk.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gwg.fehbvm.com

TS:   Math.floor(Date.now() / 1000)
来源：http://duh.jinqigufen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rdh.sweek.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ccq.zhengqikj.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lpd.jqgufenzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://imo.hnqzz.top

[J05] 时间加减（加 7 天）
来源：http://gag.tanke756.top

Py:   now + timedelta(days=7)
来源：http://rxd.zhaomingkeji.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://jqo.dashuyun.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sxe.birdmap.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lii.jqgufenzy.top

Java: LocalDate.now().plusDays(7)
来源：http://qan.yj20258.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eip.xinyue.icu

Ruby: Time.now + 7 * 86400
来源：http://ukj.hcnkem.com

C#:   DateTime.Now.AddDays(7)
来源：http://fta.cashguo.top

[J06] 计算两时间之差
来源：http://dfj.gzhubu.top

Py:   (end - start).total_seconds()
来源：http://cad.feifeiyinyue.top

PHP:  $end->diff($start)->days;
来源：http://pjf.uphjek.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://krd.gogol.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nes.ybcxt.top

Java: Duration.between(start, end).toSeconds()
来源：http://tnd.fehbvm.com

Go:   end.Sub(start).Hours()
来源：http://fiu.iojbl.cn

Ruby: end - start                 # 返回秒数
来源：http://nhk.cqqwz.cn

C#:   (end - start).TotalSeconds
来源：http://mag.fktsv.cn

[J07] 比较两个日期
来源：http://dih.9152youxi.cn

Py:   d1 < d2;  d1 == d2
来源：http://sgr.c1oappe.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dqv.xuanzx.com

JS:   d1.getTime() < d2.getTime()
来源：http://wdy.ivvv.top

TS:   d1.getTime() < d2.getTime()
来源：http://daf.xylfe.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://inl.sweek.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dax.yvedp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yoi.vehdjk.com

C#:   d1 < d2;  d1 == d2
来源：http://hrm.52xcode.cn

[J08] 提取年月日与星期
来源：http://qkn.yanxiufei.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pwm.svipenyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mbq.xylfe.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://aam.jinyuanbaomall.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bqj.tanke756.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hzj.yangfankeji.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bml.sysykeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aat.epnwcf.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zdf.52xcode.cn

[J09] 时区处理
来源：http://gcr.jinqigfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hdb.sysykeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ylk.yuxming.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gux.mhx1999.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sxc.xingfuxueyuan.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dca.smart0.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oik.jianghu66.top

Ruby: Time.now.getlocal("+08:00")
来源：http://txw.havefunace.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ino.jqgufenzy.top

[J10] 取今天 / 本月第一天
来源：http://onq.wangshuangyany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://sbg.jianghu66.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://aby.ppjwa.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zfp.shanyushiyangtech.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iis.ybcxt.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dxg.vqdsnc.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uod.feifeiyinyue.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fuw.epnwcf.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ixz.jqgufenzy.top

================================================================================
来源：http://vue.yuxming.cn

K. JSON 与序列化
来源：http://zsu.fehbvm.com

================================================================================
来源：http://qhe.zhoulong.xyz

[K01] 对象转 JSON 字符串
来源：http://sjz.jiagoushi.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hgf.yuanzhike.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lih.jinqigfzy.top

JS:   JSON.stringify(obj)
来源：http://xwe.52xcode.cn

TS:   JSON.stringify(obj)
来源：http://pcy.xylfe.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xjt.ppjwa.cn

Go:   json.Marshal(obj)
来源：http://pqs.pengpengdd.cyou

Ruby: obj.to_json                                     // require "json"
来源：http://uby.hnxiangtu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://aal.gotoacloud.top

[K02] JSON 字符串转对象
来源：http://vad.bbcook.cn

Py:   json.loads(s)
来源：http://mhx.birdmap.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wyy.nanxuanxn.top

JS:   JSON.parse(s)
来源：http://btr.snrcjt.cn

TS:   JSON.parse(s)
来源：http://hzh.hnxiangtu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jwi.wangdashe.top

Go:   json.Unmarshal(data, &v)
来源：http://vzr.jiagoushi.top

Ruby: JSON.parse(s)
来源：http://oez.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://glp.yongpay.top

[K03] JSON 美化输出（带缩进）
来源：http://syl.yvedp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wop.hfpthk.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yoa.xuanzx.com

JS:   JSON.stringify(obj, null, 2)
来源：http://cyg.hcnkem.com

TS:   JSON.stringify(obj, null, 2)
来源：http://bct.jqgufenzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xai.zhengqikj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zql.cqqwz.cn

Ruby: JSON.pretty_generate(obj)
来源：http://poe.cqqwz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qgn.iojbl.cn

[K04] 读取 JSON 文件
来源：http://kwk.chenzaomai.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dmw.ydjk.org.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yrt.bjfxy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yjv.sweek.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mvt.yongpay.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://crq.yongpay.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://umu.snrcjt.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://egz.ivvv.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oii.snrcjt.cn

[K05] 深拷贝对象
来源：http://hwt.redwolf501.top

Py:   copy.deepcopy(obj)
来源：http://loe.nanxuanxn.top

PHP:  unserialize(serialize($obj));
来源：http://ube.hesvh.cn

JS:   structuredClone(obj)
来源：http://yiu.zhixingplan.top

TS:   structuredClone(obj)
来源：http://kyj.bjfxy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://qdo.c1oappe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://njz.hongshengwenyu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wdb.fehbvm.com

C#:   // 序列化往返，或自定义 Clone
来源：http://heq.zhijiandao.cn

[K06] 解析 URL 查询串
来源：http://iny.shangyingyoupin.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jib.ydjk.org.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jix.hfpthk.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nlb.52xcode.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tvd.epnwcf.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://stz.tarul.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hcn.nwbrower.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zjc.hnqzz.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rmw.zhaomingkeji.xyz

[K07] 进制转换
来源：http://bck.zdbjq.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lau.vqdsnc.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ksv.zhoulong.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hnt.zycfv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://eqx.xinyue.icu

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ndm.hammf.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iow.tanke756.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wmj.vehdjk.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oko.andypj.xyz

[K08] 二进制序列化（非 JSON）
来源：http://lfy.sysykeji.top

Py:   pickle.dumps(obj)
来源：http://vvp.xuetiantiany.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://quo.fengsongda.top

JS:   v8.serialize(obj)        // Node
来源：http://yiq.zhijiandao.cn

TS:   v8.serialize(obj)        // Node
来源：http://mvz.cashguo.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pkp.yj20258888.top

Go:   encoding/gob
来源：http://dua.zhengqikj.top

Ruby: Marshal.dump(obj)
来源：http://gbh.xziqi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://slm.zycfv.cn

================================================================================
来源：http://fez.jinyuanbaomall.cn

L. 网络请求
来源：http://pti.fktsv.cn

================================================================================
来源：http://psb.yj20258.top

[L01] 发送 GET 请求
来源：http://mrm.c1oappe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bhy.tarul.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lia.zycfv.cn

JS:   await fetch(url)
来源：http://ukw.tian-w.cn

TS:   await fetch(url)
来源：http://ybl.tian-w.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rag.smart0.xyz

Go:   resp, err := http.Get(url)
来源：http://alh.wangdashe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://txu.pengpengdd.cyou

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iay.xuetiantiany.cn

[L02] 发送 POST JSON
来源：http://jiu.redwolf501.top

Py:   requests.post(url, json={"a": 1})
来源：http://nun.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kyq.ywan-chungtsiang.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wmp.jinqigufen.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://izh.aizwys.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://aeq.xuetiantiany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aoi.iojbl.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dnq.mhx1999.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rur.aizwys.cn

[L03] 设置自定义请求头
来源：http://xoo.smart0.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sov.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vte.redwolf501.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://alf.aizwys.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zad.yanxiufei.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://adf.yuxming.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ulg.shanyushiyangkeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fio.gogol.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cxv.xuetiantiany.cn

[L04] 设置超时
来源：http://npk.wangshuangyany.cn

Py:   requests.get(url, timeout=5)
来源：http://avm.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nsz.cheryme.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lkv.kuanghao11.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kdy.snrcjt.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hwz.ctjpmb.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dgx.hesvh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jqw.cashguo.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://otb.vehdjk.com

[L05] 上传文件（multipart）
来源：http://drc.bjfxy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ymf.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cwr.shangyingyoupin.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kko.jinqigufen.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fvc.yj20258.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://akv.yonumen.top


<!-- 参考信息 -->