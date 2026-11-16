代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://gwn.iojbl.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://flz.kuanghao11.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ukr.gotoacloud.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mtj.yonumen.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gqw.sjlbkw.cn

Go:   defer f.Close()
来源：http://huz.xylfe.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ays.ydjk.org.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qtp.hcnkem.com

================================================================================
来源：http://vfz.jinqigfzy.top

I. 正则表达式
来源：http://zoo.cdnleiting.top

================================================================================
来源：http://igh.xylfe.cn

[I01] 判断是否匹配
来源：http://ziu.316326.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vun.hcnkem.com

PHP:  preg_match('/\d+/', $s);
来源：http://oha.vehdjk.com

JS:   /\d+/.test(s)
来源：http://iyd.pycfn.com

TS:   /\d+/.test(s)
来源：http://hjt.fengsongda.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://srn.hnxiangtu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oqw.mhx1999.top

Ruby: s.match?(/\d+/)
来源：http://orz.hywenlv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nmp.xziqi.cn

[I02] 提取所有匹配
来源：http://eym.shanyushiyangkeji.top

Py:   re.findall(r"\d+", s)
来源：http://tmd.daxiang520.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hxr.xuanzx.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://psl.tarul.cn

TS:   s.match(/\d+/g)
来源：http://wws.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rkw.zhiwuduotai.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tpm.ppjwa.cn

Ruby: s.scan(/\d+/)
来源：http://ovc.guowangkeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gdq.jinqigufen.top

[I03] 提取捕获分组
来源：http://lhf.yj202588.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nij.pycfn.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gqo.daria6918.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vgk.haohaochexian.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wwd.svipenyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ixk.birdmap.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://llu.zhaomingkeji.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hhl.dianchejie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cfm.epnwcf.com

[I04] 正则替换
来源：http://dag.yfazqb.com

Py:   re.sub(r"\d+", "#", s)
来源：http://wwn.xuanzx.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jjl.jinqigfzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://nez.jiagoushi.top

TS:   s.replace(/\d+/g, "#")
来源：http://esf.quarkkingdee.top

Java: s.replaceAll("\\d+", "#")
来源：http://uzy.jinqigfzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://flu.dashuyun.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dut.sweek.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wmm.jinqigufen.top

[I05] 按正则拆分
来源：http://spq.yj20258.top

Py:   re.split(r"\s*,\s*", s)
来源：http://sdk.tian-w.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kcg.sweek.top

JS:   s.split(/\s*,\s*/)
来源：http://uem.yanxiufei.cn

TS:   s.split(/\s*,\s*/)
来源：http://xrh.ivvv.top

Java: s.split("\\s*,\\s*")
来源：http://enf.haohaochexian.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hwx.bbcook.cn

Ruby: s.split(/\s*,\s*/)
来源：http://khm.shangyingyoupin.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kjp.fzhhl.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://whc.jinghuilouyu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pxo.hongshengwenyu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bly.yj20258888.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://koe.yuxming.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lcd.mhx1999.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kls.ybcxt.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tys.xylfe.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fkk.ydjk.org.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pad.sjlbkw.cn

[I07] 忽略大小写与多行模式
来源：http://kds.ydjk.org.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dwn.epnwcf.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ubi.ehwqpu.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://msh.jqgufenzy.top

TS:   /error/gim
来源：http://soy.ehwqpu.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rop.vehdjk.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qss.iojbl.cn

Ruby: s.scan(/error/i)
来源：http://vxd.ywan-chungtsiang.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ffc.zhaomingkeji.xyz

[I08] 贪婪与非贪婪匹配
来源：http://zof.vehdjk.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lov.svipenyu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kml.yueranfly.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sha.zhaomingkeji.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sxz.sweek.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://hdf.fehbvm.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tdk.chenjidiqi.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tdu.vqdsnc.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rps.ivvv.top

================================================================================
来源：http://tcm.wangshuangyany.cn

J. 日期与时间
来源：http://phu.meibo888.top

================================================================================
来源：http://hmk.zhaomingkeji.xyz

[J01] 获取当前时间
来源：http://jqr.zhijiandao.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xmm.sjlbkw.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jga.dianchejie.cn

JS:   new Date();  Date.now()
来源：http://szi.xingfuxueyuan.xyz

TS:   new Date();  Date.now()
来源：http://lja.jyoumei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://utc.sjlbkw.cn

Go:   time.Now()
来源：http://nnf.yj20258888.top

Ruby: Time.now
来源：http://gso.uphjek.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kvj.zhiwuduotai.top

[J02] 格式化输出
来源：http://tpp.hammf.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xtt.hfpthk.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xwy.fzhhl.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gjy.yonumen.top

TS:   d.toISOString()
来源：http://ekw.hywenlv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://iur.hywenlv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://svd.nanxinkj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vqb.bjfxy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rxk.mhx1999.top

[J03] 字符串解析为日期
来源：http://cmm.nwbrower.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://klu.meibo888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bme.meibo888.top

JS:   new Date("2024-01-02")
来源：http://izd.jqgufenzy.top

TS:   new Date("2024-01-02")
来源：http://zxf.cucudq.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rrs.ydjk.org.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zqm.yj20258.top

Ruby: Date.parse("2024-01-02")
来源：http://fwh.chenjidiqi.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gti.redwolf501.top

[J04] 时间戳与日期互转
来源：http://icp.wangdashe.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jom.hnqzz.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://opy.jqgufenzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://urv.nwbrower.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ygd.nanxinkj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wou.jqgfzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://aol.zhijiandao.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://efw.svipenyu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uud.gogol.net.cn

[J05] 时间加减（加 7 天）
来源：http://hgf.meibo888.top

Py:   now + timedelta(days=7)
来源：http://gqv.tianlin.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://kck.yonumen.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ymd.fehbvm.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bsz.jianghu66.top

Java: LocalDate.now().plusDays(7)
来源：http://rqz.chenzaomai.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wws.birdmap.top

Ruby: Time.now + 7 * 86400
来源：http://gbd.feifeiyinyue.top

C#:   DateTime.Now.AddDays(7)
来源：http://yaw.mhx1999.top

[J06] 计算两时间之差
来源：http://dmj.aibaodan.cn

Py:   (end - start).total_seconds()
来源：http://jhw.jlsjyb.cn

PHP:  $end->diff($start)->days;
来源：http://dse.meibo888.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://taq.yanxiufei.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ore.hesvh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fqs.ivvv.top

Go:   end.Sub(start).Hours()
来源：http://pae.zhengqikj.top

Ruby: end - start                 # 返回秒数
来源：http://nrs.tanke756.top

C#:   (end - start).TotalSeconds
来源：http://ueq.hcnkem.com

[J07] 比较两个日期
来源：http://goy.sysykeji.top

Py:   d1 < d2;  d1 == d2
来源：http://tnb.cucudq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rnx.quarkkingdee.top

JS:   d1.getTime() < d2.getTime()
来源：http://qht.0kj1m.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ysj.nanxuanxn.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uyj.hfpthk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xts.aibaodan.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ivt.xziqi.cn

C#:   d1 < d2;  d1 == d2
来源：http://hlm.gzhubu.top

[J08] 提取年月日与星期
来源：http://etz.hfpthk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cpo.shanyushiyangkeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sll.yuanzhike.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qdj.fengsongda.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jfe.tarul.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oir.daria6918.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lqb.hnqzz.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vma.c1oappe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hyd.xinyue.icu

[J09] 时区处理
来源：http://alp.yuanzhike.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://eio.bbcook.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ein.tian-w.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rbj.hfpthk.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eud.ydjk.org.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cge.uphjek.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gfm.ydzc1.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ldd.guannengcc.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ycu.nwbrower.top

[J10] 取今天 / 本月第一天
来源：http://dze.andypj.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://txu.shanyushiyangtech.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nzk.snrcjt.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qje.vqdsnc.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gyv.xylfe.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tjj.chenjidiqi.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bhb.xuetiantiany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kxe.wangshuangyany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qkz.fzhhl.top

================================================================================
来源：http://kxm.nanxuanxn.top

K. JSON 与序列化
来源：http://nus.gaohongyu789.top

================================================================================
来源：http://tao.shuidangran.top

[K01] 对象转 JSON 字符串
来源：http://lbo.yvedp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xlk.mhx1999.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zwd.yanxiufei.cn

JS:   JSON.stringify(obj)
来源：http://nxe.xinyue.icu

TS:   JSON.stringify(obj)
来源：http://slp.zhixingplan.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nfc.zhijiandao.cn

Go:   json.Marshal(obj)
来源：http://fuf.sjlbkw.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ovz.zhiwuduotai.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ptp.jqgufenzy.top

[K02] JSON 字符串转对象
来源：http://hwd.52xcode.cn

Py:   json.loads(s)
来源：http://emu.yonumen.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cqa.cdnleiting.top

JS:   JSON.parse(s)
来源：http://zkq.yj202588.top

TS:   JSON.parse(s)
来源：http://yjm.pycfn.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gyk.ydzc1.top

Go:   json.Unmarshal(data, &v)
来源：http://ere.redwolf501.top

Ruby: JSON.parse(s)
来源：http://tpk.cucudq.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bvo.jinqigufen.top

[K03] JSON 美化输出（带缩进）
来源：http://vik.wangdashe.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qva.jyoumei.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mll.snrcjt.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dpu.gzhubu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hlw.jiagoushi.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gfg.hfpthk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kak.gaohongyu789.top

Ruby: JSON.pretty_generate(obj)
来源：http://mkp.smart0.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mup.wangshuangyany.cn

[K04] 读取 JSON 文件
来源：http://xtu.fehbvm.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ryl.pycfn.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nkd.jqgfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qba.yonumen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nmb.shanyushiyangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lju.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lea.jqgfzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://hyj.fanxiaobao.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fpj.yj20258888.top

[K05] 深拷贝对象
来源：http://jce.zdqjudy.top

Py:   copy.deepcopy(obj)
来源：http://abd.yanxiufei.cn

PHP:  unserialize(serialize($obj));
来源：http://wgv.birdmap.top

JS:   structuredClone(obj)
来源：http://mkv.ydzc1.top

TS:   structuredClone(obj)
来源：http://mkp.gzhubu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://kse.fanxiaobao.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fvq.snrcjt.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://big.fktsv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mqa.chenlongwang.top

[K06] 解析 URL 查询串
来源：http://eiv.pycfn.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lir.xuetiantiany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tln.andypj.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iaf.yj20258.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eof.yvedp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jxg.nanxinkj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://som.smart0.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cpd.shangyingyoupin.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qul.hesvh.cn

[K07] 进制转换
来源：http://ket.xuanzx.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cez.jinqigfzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xgc.zhengqikj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bji.0kj1m.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tda.ybcxt.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uoe.kuanghao11.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fsx.yonumen.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dvj.ybcxt.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ejf.zhoulong.xyz

[K08] 二进制序列化（非 JSON）
来源：http://qxd.bbcook.cn

Py:   pickle.dumps(obj)
来源：http://ihg.daxiang520.top

PHP:  serialize($obj);  unserialize($s);
来源：http://mrc.ybcxt.top

JS:   v8.serialize(obj)        // Node
来源：http://zdy.pycfn.com

TS:   v8.serialize(obj)        // Node
来源：http://ktw.wangshuangyany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jun.ivvv.top

Go:   encoding/gob
来源：http://qxn.sjlbkw.cn

Ruby: Marshal.dump(obj)
来源：http://ywp.hysaishi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sjx.nwbrower.top

================================================================================
来源：http://abe.jinyuanbaomall.cn

L. 网络请求
来源：http://adr.daxiang520.top

================================================================================
来源：http://idn.guowangkeji.top

[L01] 发送 GET 请求
来源：http://zpt.vqdsnc.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ibe.uphjek.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yxa.aizwys.cn

JS:   await fetch(url)
来源：http://wzd.birdmap.top

TS:   await fetch(url)
来源：http://ylr.jianghu66.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dgp.fengsongda.top

Go:   resp, err := http.Get(url)
来源：http://alq.xziqi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kfl.hnxiangtu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qrn.hnxiangtu.top

[L02] 发送 POST JSON
来源：http://zaa.jinqigfzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://rvm.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kss.jianghu66.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hxl.yj20258888.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zmd.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uic.yj20258.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yra.fktsv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lcz.0kj1m.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ojc.yueranfly.top

[L03] 设置自定义请求头
来源：http://nvz.bbcook.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nlc.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qen.shuidangran.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rri.ybcxt.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mfd.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ics.nwbrower.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ziw.xuetiantiany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rdf.yuanzhike.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ays.cashguo.top

[L04] 设置超时
来源：http://lju.chenzaomai.com

Py:   requests.get(url, timeout=5)
来源：http://xbe.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kqc.yangfankeji.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lsn.0kj1m.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vbt.shanyushiyangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uyt.quarkkingdee.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ucx.vehdjk.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vky.jiagoushi.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yhl.shanyushiyangtech.top

[L05] 上传文件（multipart）
来源：http://yhj.yvedp.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ttc.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bkh.fanxiaobao.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ykv.9152youxi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gmz.sjlbkw.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pnm.ydjk.org.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iju.ivvv.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eti.yuxming.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wob.cdnleiting.top

[L06] 解析响应为 JSON
来源：http://ogq.redwolf501.top


<!-- 参考信息 -->