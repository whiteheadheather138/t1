代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://qjr.gzhubu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jvj.jinyuanbaomall.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hhl.shuidangran.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bbz.kuanghao11.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yih.shanyushiyangtech.top

Go:   defer f.Close()
来源：http://htd.chenjidiqi.icu

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ojk.uphjek.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ouo.quarkkingdee.top

================================================================================
来源：http://rcz.cqqwz.cn

I. 正则表达式
来源：http://srs.vehdjk.com

================================================================================
来源：http://mxv.jlsjyb.cn

[I01] 判断是否匹配
来源：http://iqt.jianghu66.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zgq.hfpthk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lfh.kuanghao11.cn

JS:   /\d+/.test(s)
来源：http://wiv.daxiang520.top

TS:   /\d+/.test(s)
来源：http://nrd.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xph.yueranfly.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jos.ydzc1.top

Ruby: s.match?(/\d+/)
来源：http://waw.yanxiufei.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cgk.jqgufenzy.top

[I02] 提取所有匹配
来源：http://mbn.zhaomingkeji.xyz

Py:   re.findall(r"\d+", s)
来源：http://fyb.xziqi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cku.guannengcc.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jwg.tianlin.xyz

TS:   s.match(/\d+/g)
来源：http://dbp.yueranfly.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://shm.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oia.yongpay.top

Ruby: s.scan(/\d+/)
来源：http://uex.hesvh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yvl.fanxiaobao.xyz

[I03] 提取捕获分组
来源：http://xtz.yongpay.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://exl.cqqwz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nwy.shzxlz.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gmm.jinqigufen.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bmp.hysaishi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zva.hnqzz.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mpg.xinyue.icu

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lyv.aizwys.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://smd.meibo888.top

[I04] 正则替换
来源：http://jgq.shanyushiyangtech.top

Py:   re.sub(r"\d+", "#", s)
来源：http://lfw.zhaomingkeji.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fdt.jqgfzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://uni.xingfuxueyuan.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://kng.ppjwa.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ker.cqqwz.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://spi.hnxiangtu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://twv.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jhu.cheryme.top

[I05] 按正则拆分
来源：http://hhc.jyoumei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qhj.9152youxi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tgy.haohaochexian.top

JS:   s.split(/\s*,\s*/)
来源：http://znm.xinyue.icu

TS:   s.split(/\s*,\s*/)
来源：http://yjx.sufxvd.cn

Java: s.split("\\s*,\\s*")
来源：http://oqr.ppjwa.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ftz.yanxiufei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hgx.yangfankeji.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gep.zhengqikj.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://eom.kuanghao11.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ozp.gogol.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cjf.cqqwz.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://krj.sjlbkw.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hkk.gotoacloud.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bfy.gotoacloud.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ufu.zhiwuduotai.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uzk.cashguo.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wps.jinghuilouyu.cn

[I07] 忽略大小写与多行模式
来源：http://qyk.aizwys.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iei.fanxiaobao.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jvt.vehdjk.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kmp.zdqjudy.top

TS:   /error/gim
来源：http://jvp.ydzc1.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tbb.zhixingplan.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zja.tianlin.xyz

Ruby: s.scan(/error/i)
来源：http://qkc.tarul.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cwq.fanxiaobao.xyz

[I08] 贪婪与非贪婪匹配
来源：http://uyj.9152youxi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uue.tianlin.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vnj.aizwys.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zdc.ppjwa.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://laq.daxiang520.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://lou.tanke756.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lhm.uphjek.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yms.havefunace.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ink.andypj.xyz

================================================================================
来源：http://eqt.jqgfzy.top

J. 日期与时间
来源：http://omq.kuanghao11.cn

================================================================================
来源：http://wag.xingfuxueyuan.xyz

[J01] 获取当前时间
来源：http://vtu.epnwcf.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://zdf.yanxiufei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lme.sjlbkw.cn

JS:   new Date();  Date.now()
来源：http://ubt.cdnleiting.top

TS:   new Date();  Date.now()
来源：http://bnp.daria6918.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dkv.kuanghao11.cn

Go:   time.Now()
来源：http://bvx.hywenlv.cn

Ruby: Time.now
来源：http://knq.zhengqikj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://apk.zdqjudy.top

[J02] 格式化输出
来源：http://egi.dashuyun.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mcc.hfpthk.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yyd.fzhhl.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fwm.xingfuxueyuan.xyz

TS:   d.toISOString()
来源：http://bkr.shangyingyoupin.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sti.cheryme.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://iok.snrcjt.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ikd.jinghuilouyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://slk.sweek.top

[J03] 字符串解析为日期
来源：http://grt.hesvh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://efi.vqdsnc.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ssj.tarul.cn

JS:   new Date("2024-01-02")
来源：http://doi.chenjidiqi.icu

TS:   new Date("2024-01-02")
来源：http://pce.nanxinkj.top

Java: LocalDate.parse("2024-01-02")
来源：http://ddp.nanxuanxn.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jap.fehbvm.com

Ruby: Date.parse("2024-01-02")
来源：http://cmw.fengsongda.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://evj.tarul.cn

[J04] 时间戳与日期互转
来源：http://zhg.vqdsnc.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iqt.aizwys.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kee.mhx1999.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://emy.wangdashe.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jhl.jianghu66.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dbt.havefunace.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uct.meibo888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hyh.cucudq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://snf.zhongyouzk.top

[J05] 时间加减（加 7 天）
来源：http://itd.snrcjt.cn

Py:   now + timedelta(days=7)
来源：http://mdx.pengpengdd.cyou

PHP:  (new DateTime())->modify("+7 days");
来源：http://cad.zhoulong.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dht.gotoacloud.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wvi.pengpengdd.cyou

Java: LocalDate.now().plusDays(7)
来源：http://rdq.yvedp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://msi.aibaodan.cn

Ruby: Time.now + 7 * 86400
来源：http://ywq.yuxming.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xrt.redwolf501.top

[J06] 计算两时间之差
来源：http://smi.yj20258.top

Py:   (end - start).total_seconds()
来源：http://vth.xuanzx.com

PHP:  $end->diff($start)->days;
来源：http://whb.shangyingyoupin.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ayw.yonumen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pim.yfazqb.com

Java: Duration.between(start, end).toSeconds()
来源：http://lpl.cucudq.cn

Go:   end.Sub(start).Hours()
来源：http://cad.xingfuxueyuan.xyz

Ruby: end - start                 # 返回秒数
来源：http://ieb.hammf.cn

C#:   (end - start).TotalSeconds
来源：http://jgb.jinqigufen.top

[J07] 比较两个日期
来源：http://url.fehbvm.com

Py:   d1 < d2;  d1 == d2
来源：http://njs.0kj1m.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lqm.yvedp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://biv.guowangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://gel.ybcxt.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vcs.fanxiaobao.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ipx.andypj.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://pff.zhixingplan.top

C#:   d1 < d2;  d1 == d2
来源：http://fzf.feifeiyinyue.top

[J08] 提取年月日与星期
来源：http://qjv.birdmap.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wuq.epnwcf.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://whf.yangfankeji.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xdw.c1oappe.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ixq.hongshengwenyu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ofr.shangyingyoupin.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://siy.dianchejie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bie.iojbl.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cse.jinqigfzy.top

[J09] 时区处理
来源：http://rzz.hfpthk.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://iwy.aizwys.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ptm.xziqi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fmr.shangyingyoupin.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://auw.haohaochexian.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uhk.yangfankeji.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ltp.zhijiandao.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wiy.fzhhl.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bfx.zhaomingkeji.xyz

[J10] 取今天 / 本月第一天
来源：http://vwk.zhiwuduotai.top

Py:   date.today();  date.today().replace(day=1)
来源：http://oaa.zhixingplan.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zad.jianghu66.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qlh.chenlongwang.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zaf.shzxlz.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qhd.hnxiangtu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://spz.ivvv.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gic.jyoumei.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rno.vehdjk.com

================================================================================
来源：http://vxi.fehbvm.com

K. JSON 与序列化
来源：http://dts.ydjk.org.cn

================================================================================
来源：http://aag.tianlin.xyz

[K01] 对象转 JSON 字符串
来源：http://xwp.hcnkem.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zfr.vehdjk.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gok.feifeiyinyue.top

JS:   JSON.stringify(obj)
来源：http://ndl.zhiwuduotai.top

TS:   JSON.stringify(obj)
来源：http://wwe.pycfn.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dmi.xingfuxueyuan.xyz

Go:   json.Marshal(obj)
来源：http://vlm.ydzc1.top

Ruby: obj.to_json                                     // require "json"
来源：http://miu.haohaochexian.top

C#:   JsonSerializer.Serialize(obj)
来源：http://dcj.dianchejie.cn

[K02] JSON 字符串转对象
来源：http://des.shzxlz.cn

Py:   json.loads(s)
来源：http://xst.chenzaomai.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yjg.feifeiyinyue.top

JS:   JSON.parse(s)
来源：http://gpj.daria6918.cn

TS:   JSON.parse(s)
来源：http://ibk.havefunace.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qwt.zhaomingkeji.xyz

Go:   json.Unmarshal(data, &v)
来源：http://fwv.gogol.net.cn

Ruby: JSON.parse(s)
来源：http://tfk.zhiwuduotai.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://omx.yuxming.cn

[K03] JSON 美化输出（带缩进）
来源：http://kqh.wangshuangyany.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zen.quarkkingdee.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://msp.gzhubu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://uqo.xuetiantiany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://epn.sjlbkw.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://isq.wangdashe.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://njt.xingfuxueyuan.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://wtp.hnqzz.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nrb.chenjidiqi.icu

[K04] 读取 JSON 文件
来源：http://idt.chenjidiqi.icu

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://max.jinqigfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bdy.hysaishi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qcg.aibaodan.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qgt.yongpay.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mgo.wangdashe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qms.zhijiandao.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fyu.bbcook.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jlx.iojbl.cn

[K05] 深拷贝对象
来源：http://viz.fanxiaobao.xyz

Py:   copy.deepcopy(obj)
来源：http://ewm.jyoumei.cn

PHP:  unserialize(serialize($obj));
来源：http://mhu.yuanzhike.top

JS:   structuredClone(obj)
来源：http://ecd.xinyue.icu

TS:   structuredClone(obj)
来源：http://ntj.xuetiantiany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ubl.zhijiandao.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ogq.zhoulong.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nnf.shanyushiyangtech.top

C#:   // 序列化往返，或自定义 Clone
来源：http://snp.0kj1m.cn

[K06] 解析 URL 查询串
来源：http://yzy.ctjpmb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wms.yanxiufei.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mcg.xuetiantiany.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wtc.ydzc1.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dis.jianghu66.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wva.guowangkeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://pjj.ehwqpu.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vua.xinyue.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vdo.yueranfly.top

[K07] 进制转换
来源：http://xuv.yanxiufei.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nqo.redwolf501.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://msz.yvedp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qxw.ppjwa.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dww.tianlin.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://azf.ydzc1.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hwk.ybcxt.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vlr.jinqigufen.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uap.shanyushiyangtech.top

[K08] 二进制序列化（非 JSON）
来源：http://gli.zdbjq.cn

Py:   pickle.dumps(obj)
来源：http://fjm.jiagoushi.top

PHP:  serialize($obj);  unserialize($s);
来源：http://tkw.hysaishi.cn

JS:   v8.serialize(obj)        // Node
来源：http://cdv.chenzaomai.com

TS:   v8.serialize(obj)        // Node
来源：http://pxb.pycfn.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://azo.pycfn.com

Go:   encoding/gob
来源：http://ygu.wangdashe.top

Ruby: Marshal.dump(obj)
来源：http://xkw.iojbl.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ijh.cucudq.cn

================================================================================
来源：http://hmr.hfpthk.cn

L. 网络请求
来源：http://rfi.zhiwuduotai.top

================================================================================
来源：http://crl.ydzc1.top

[L01] 发送 GET 请求
来源：http://fnj.hcnkem.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gha.nanxuanxn.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uig.cucudq.cn

JS:   await fetch(url)
来源：http://ujs.chenlongwang.top

TS:   await fetch(url)
来源：http://pvc.xuetiantiany.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sle.jinghuilouyu.cn

Go:   resp, err := http.Get(url)
来源：http://foq.sxryk.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qjr.zhixingplan.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uao.sweek.top

[L02] 发送 POST JSON
来源：http://kgr.bjfxy.top

Py:   requests.post(url, json={"a": 1})
来源：http://dlv.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://glg.andypj.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fne.fanxiaobao.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://syg.guannengcc.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rdx.xuanzx.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cqo.jiagoushi.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lta.sufxvd.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dmu.shanyushiyangtech.top

[L03] 设置自定义请求头
来源：http://rtt.yfazqb.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://itl.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://psi.ctjpmb.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cdy.wangdashe.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ufc.zhoulong.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://iuf.zhengqikj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ush.cdnleiting.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oyy.zhengqikj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mfb.ywan-chungtsiang.top

[L04] 设置超时
来源：http://bkk.bjfxy.top

Py:   requests.get(url, timeout=5)
来源：http://vfy.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xeq.tian-w.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qrs.tianlin.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://utv.52xcode.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://szf.yueranfly.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pfg.dianchejie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://loz.vqdsnc.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xrz.jinqigufen.top

[L05] 上传文件（multipart）
来源：http://nfr.hnxiangtu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hnx.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hoq.ppjwa.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qjk.mhx1999.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lne.c1oappe.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mze.zhongyouzk.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://euq.fengsongda.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vlu.nwbrower.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://epe.vehdjk.com

[L06] 解析响应为 JSON
来源：http://hqk.sweek.top


<!-- 参考信息 -->