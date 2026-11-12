代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://poi.quarkkingdee.top

Ruby: raise MyError.new("fail", 500)
来源：http://nas.jinqigfzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://oqq.cashguo.top

[H10] 资源自动释放
来源：http://xyp.nanxinkj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://yca.shanyushiyangkeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://btw.shanyushiyangkeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ifs.jqgufenzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://eus.gaohongyu789.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://squ.hnxiangtu.top

Go:   defer f.Close()
来源：http://xig.ydjk.org.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://opp.zhoulong.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zqr.ppjwa.cn

================================================================================
来源：http://mgl.meibo888.top

I. 正则表达式
来源：http://cis.yonumen.top

================================================================================
来源：http://trd.zhoulong.xyz

[I01] 判断是否匹配
来源：http://iex.jinghuilouyu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://swl.wangshuangyany.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ivt.uphjek.com

JS:   /\d+/.test(s)
来源：http://ioo.guannengcc.top

TS:   /\d+/.test(s)
来源：http://fqf.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dra.52xcode.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rzk.zhiwuduotai.top

Ruby: s.match?(/\d+/)
来源：http://obn.nwbrower.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://upa.shangyingyoupin.top

[I02] 提取所有匹配
来源：http://mho.hesvh.cn

Py:   re.findall(r"\d+", s)
来源：http://rqd.dianchejie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sdc.daria6918.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gdf.shanyushiyangtech.top

TS:   s.match(/\d+/g)
来源：http://scr.meibo888.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nhu.yj20258.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yie.sweek.top

Ruby: s.scan(/\d+/)
来源：http://vag.andypj.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://epj.yj202588.top

[I03] 提取捕获分组
来源：http://aiw.fengsongda.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qrn.hfpthk.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jvv.xingfuxueyuan.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yzg.ivvv.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kid.52xcode.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sxo.sxryk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jkn.hnqzz.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nxd.zdbjq.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vet.zdbjq.cn

[I04] 正则替换
来源：http://rmk.hesvh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tzk.andypj.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fii.hywenlv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tep.guowangkeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://mfi.gotoacloud.top

Java: s.replaceAll("\\d+", "#")
来源：http://kte.jianghu66.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wlt.bbcook.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hrd.9152youxi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kvs.sxryk.cn

[I05] 按正则拆分
来源：http://xli.yongpay.top

Py:   re.split(r"\s*,\s*", s)
来源：http://cmz.xuanzx.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gpm.yangfankeji.com

JS:   s.split(/\s*,\s*/)
来源：http://lgp.zdbjq.cn

TS:   s.split(/\s*,\s*/)
来源：http://inc.wangshuangyany.cn

Java: s.split("\\s*,\\s*")
来源：http://hfk.sweek.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dfv.c1oappe.top

Ruby: s.split(/\s*,\s*/)
来源：http://kxi.jinqigfzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sia.nanxinkj.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://axn.smart0.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xmj.pycfn.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yjj.chenlongwang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yoe.bjfxy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wcs.vqdsnc.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lmk.ehwqpu.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://laz.jinqigfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bpx.yongpay.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vif.hnxiangtu.top

[I07] 忽略大小写与多行模式
来源：http://phd.kuanghao11.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bhe.redwolf501.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dac.hnqzz.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vow.zhijiandao.cn

TS:   /error/gim
来源：http://mci.ppjwa.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ipn.yj202588.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://exj.svipenyu.cn

Ruby: s.scan(/error/i)
来源：http://ppa.c1oappe.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dmr.zhongyouzk.top

[I08] 贪婪与非贪婪匹配
来源：http://jvz.xuanzx.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gde.sxryk.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nud.meibo888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ija.cdnleiting.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://guh.bjfxy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://aou.zhongyouzk.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dbo.meibo888.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vvo.mhx1999.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qxl.zhaomingkeji.xyz

================================================================================
来源：http://lub.jyoumei.cn

J. 日期与时间
来源：http://tza.cheryme.top

================================================================================
来源：http://aac.zhixingplan.top

[J01] 获取当前时间
来源：http://ecg.tianlin.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://acf.sjlbkw.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uxe.ydzc1.top

JS:   new Date();  Date.now()
来源：http://grl.jiagoushi.top

TS:   new Date();  Date.now()
来源：http://atg.uphjek.com

Java: LocalDateTime.now();  Instant.now()
来源：http://muz.yonumen.top

Go:   time.Now()
来源：http://avl.jiagoushi.top

Ruby: Time.now
来源：http://atr.epnwcf.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://klj.zdqjudy.top

[J02] 格式化输出
来源：http://ekj.snrcjt.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rup.cucudq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fbn.zhixingplan.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mwu.daria6918.cn

TS:   d.toISOString()
来源：http://jqu.feifeiyinyue.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rwd.yvedp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bgl.cdnleiting.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zbl.sxryk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xlr.tian-w.cn

[J03] 字符串解析为日期
来源：http://zbd.zhongyouzk.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ryu.zdqjudy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ixz.bbcook.cn

JS:   new Date("2024-01-02")
来源：http://mit.fehbvm.com

TS:   new Date("2024-01-02")
来源：http://pdf.chenzaomai.com

Java: LocalDate.parse("2024-01-02")
来源：http://sjb.daria6918.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nah.ywan-chungtsiang.top

Ruby: Date.parse("2024-01-02")
来源：http://nje.ctjpmb.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://geg.xinyue.icu

[J04] 时间戳与日期互转
来源：http://jdj.tianlin.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wla.yj202588.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mac.bjfxy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://meo.pycfn.com

TS:   Math.floor(Date.now() / 1000)
来源：http://sqm.tianlin.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sjj.jqgfzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uzc.shzxlz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.gogol.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pnh.yonumen.top

[J05] 时间加减（加 7 天）
来源：http://knx.dianchejie.cn

Py:   now + timedelta(days=7)
来源：http://vjl.hywenlv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mvq.daria6918.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xyb.yj20258.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kta.ivvv.top

Java: LocalDate.now().plusDays(7)
来源：http://obm.jyoumei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mqk.haohaochexian.top

Ruby: Time.now + 7 * 86400
来源：http://xum.ydzc1.top

C#:   DateTime.Now.AddDays(7)
来源：http://dlm.nanxuanxn.top

[J06] 计算两时间之差
来源：http://ttc.birdmap.top

Py:   (end - start).total_seconds()
来源：http://nmv.aizwys.cn

PHP:  $end->diff($start)->days;
来源：http://bci.redwolf501.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://shc.ywan-chungtsiang.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://abg.jinqigufen.top

Java: Duration.between(start, end).toSeconds()
来源：http://zip.ivvv.top

Go:   end.Sub(start).Hours()
来源：http://ieh.jiagoushi.top

Ruby: end - start                 # 返回秒数
来源：http://imn.redwolf501.top

C#:   (end - start).TotalSeconds
来源：http://uqa.ctjpmb.com

[J07] 比较两个日期
来源：http://gte.zdbjq.cn

Py:   d1 < d2;  d1 == d2
来源：http://wku.zycfv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://oef.feifeiyinyue.top

JS:   d1.getTime() < d2.getTime()
来源：http://yjw.ydzc1.top

TS:   d1.getTime() < d2.getTime()
来源：http://gct.gzhubu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://exb.nwbrower.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cqh.yj20258.top

Ruby: d1 < d2;  d1 == d2
来源：http://gnh.shanyushiyangtech.top

C#:   d1 < d2;  d1 == d2
来源：http://zat.yanxiufei.cn

[J08] 提取年月日与星期
来源：http://rcn.birdmap.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hnv.chenlongwang.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dxk.jinqigfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://are.hammf.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nnu.hcnkem.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yjo.daria6918.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uhk.zhixingplan.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tur.shuidangran.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bxm.jqgufenzy.top

[J09] 时区处理
来源：http://rjr.yuxming.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pch.ctjpmb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gub.cheryme.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jiy.zycfv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cmq.yanxiufei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vdm.hcnkem.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bui.ydzc1.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hyu.hnqzz.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://moh.zycfv.cn

[J10] 取今天 / 本月第一天
来源：http://vrx.birdmap.top

Py:   date.today();  date.today().replace(day=1)
来源：http://pez.gaohongyu789.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mkd.hnqzz.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://opj.nanxinkj.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kap.sufxvd.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://edq.hnxiangtu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zwj.fehbvm.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dxk.cucudq.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://miz.ivvv.top

================================================================================
来源：http://hya.xuetiantiany.cn

K. JSON 与序列化
来源：http://ycp.xinyue.icu

================================================================================
来源：http://opq.hnxiangtu.top

[K01] 对象转 JSON 字符串
来源：http://vnl.hnxiangtu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pll.havefunace.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yua.guowangkeji.top

JS:   JSON.stringify(obj)
来源：http://ejq.0kj1m.cn

TS:   JSON.stringify(obj)
来源：http://pdb.jyoumei.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blh.tanke756.top

Go:   json.Marshal(obj)
来源：http://glp.jqgufenzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://kgr.jyoumei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lic.dianchejie.cn

[K02] JSON 字符串转对象
来源：http://bcj.yanxiufei.cn

Py:   json.loads(s)
来源：http://hmf.zhijiandao.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nmf.ivvv.top

JS:   JSON.parse(s)
来源：http://ilz.ppjwa.cn

TS:   JSON.parse(s)
来源：http://gbi.jlsjyb.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sek.yanxiufei.cn

Go:   json.Unmarshal(data, &v)
来源：http://jzl.xylfe.cn

Ruby: JSON.parse(s)
来源：http://gej.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ajt.jqgufenzy.top

[K03] JSON 美化输出（带缩进）
来源：http://fdl.nwbrower.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://icy.yangfankeji.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dlg.zhengqikj.top

JS:   JSON.stringify(obj, null, 2)
来源：http://pln.ywan-chungtsiang.top

TS:   JSON.stringify(obj, null, 2)
来源：http://agz.zhixingplan.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cab.uphjek.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jcu.gogol.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://teq.hcnkem.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uri.feifeiyinyue.top

[K04] 读取 JSON 文件
来源：http://mwb.shzxlz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qwy.sjlbkw.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://alo.snrcjt.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ofu.wangshuangyany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qnn.0kj1m.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rrn.pycfn.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bnw.redwolf501.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://hdk.chenzaomai.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oca.jiagoushi.top

[K05] 深拷贝对象
来源：http://wqa.zhoulong.xyz

Py:   copy.deepcopy(obj)
来源：http://ggm.haohaochexian.top

PHP:  unserialize(serialize($obj));
来源：http://nct.yonumen.top

JS:   structuredClone(obj)
来源：http://llf.jinyuanbaomall.cn

TS:   structuredClone(obj)
来源：http://jum.cheryme.top

Java: // 手写拷贝构造，或序列化往返
来源：http://eij.bjfxy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tnq.316326.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fdz.yfazqb.com

C#:   // 序列化往返，或自定义 Clone
来源：http://kef.jinqigufen.top

[K06] 解析 URL 查询串
来源：http://moj.xinyue.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pkv.sysykeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cts.xziqi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zge.52xcode.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xva.cdnleiting.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cdm.zhijiandao.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gck.yongpay.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wub.jinqigufen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rby.yonumen.top

[K07] 进制转换
来源：http://roo.cashguo.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://omt.yj202588.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vtb.tianlin.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pcq.guannengcc.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ytu.hysaishi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uje.yj20258.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fnz.fanxiaobao.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ggt.zhongyouzk.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://czu.guannengcc.top

[K08] 二进制序列化（非 JSON）
来源：http://dkr.fengsongda.top

Py:   pickle.dumps(obj)
来源：http://hqz.sjlbkw.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qdk.hnxiangtu.top

JS:   v8.serialize(obj)        // Node
来源：http://xbp.gaohongyu789.top

TS:   v8.serialize(obj)        // Node
来源：http://ten.yangfankeji.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://klc.ydjk.org.cn

Go:   encoding/gob
来源：http://kje.xingfuxueyuan.xyz

Ruby: Marshal.dump(obj)
来源：http://ohj.mhx1999.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cyn.yuxming.cn

================================================================================
来源：http://fhk.cdnleiting.top

L. 网络请求
来源：http://idj.vqdsnc.cn

================================================================================
来源：http://axy.cqqwz.cn

[L01] 发送 GET 请求
来源：http://bla.jinqigfzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rtz.yvedp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kzx.meibo888.top

JS:   await fetch(url)
来源：http://tmv.zhengqikj.top

TS:   await fetch(url)
来源：http://lgu.nanxinkj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ppv.yuanzhike.top

Go:   resp, err := http.Get(url)
来源：http://fdj.dianchejie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://egy.tarul.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wxn.uphjek.com

[L02] 发送 POST JSON
来源：http://pip.snrcjt.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wiw.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://whj.daxiang520.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sds.zhongyouzk.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ghc.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hzk.kuanghao11.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sts.hnxiangtu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ybw.chenlongwang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ysn.cheryme.top

[L03] 设置自定义请求头
来源：http://dpn.tarul.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kjs.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fot.birdmap.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gmk.chenzaomai.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vkb.shuidangran.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://puo.yonumen.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wcp.daria6918.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://paf.fzhhl.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zqw.daxiang520.top

[L04] 设置超时
来源：http://wqc.yuanzhike.top

Py:   requests.get(url, timeout=5)
来源：http://ivm.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mkq.havefunace.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://krl.jinyuanbaomall.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://peo.haohaochexian.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cmw.redwolf501.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nuh.tanke756.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://aac.nwbrower.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://obt.cqqwz.cn

[L05] 上传文件（multipart）
来源：http://znp.zhaomingkeji.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ona.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sap.daxiang520.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vjp.yj202588.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tnk.hesvh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sfy.ydjk.org.cn


<!-- 参考信息 -->