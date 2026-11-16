代发 wailian999

[I02] 提取所有匹配
来源：http://qhc.hywenlv.cn

Py:   re.findall(r"\d+", s)
来源：http://ipb.hongshengwenyu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wpg.shanyushiyangtech.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zoy.jiagoushi.top

TS:   s.match(/\d+/g)
来源：http://wzm.tian-w.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://frh.havefunace.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xbk.pengpengdd.cyou

Ruby: s.scan(/\d+/)
来源：http://nbx.zdbjq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://clw.yanxiufei.cn

[I03] 提取捕获分组
来源：http://kjo.dashuyun.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bgt.nwbrower.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kjz.jinyuanbaomall.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yhn.yanxiufei.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bcs.svipenyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://arh.tian-w.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dld.xylfe.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jbz.chenlongwang.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kzr.wangshuangyany.cn

[I04] 正则替换
来源：http://sjj.hfpthk.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jql.epnwcf.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://idf.hammf.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rwf.ivvv.top

TS:   s.replace(/\d+/g, "#")
来源：http://zer.dashuyun.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gle.kuanghao11.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dmh.ppjwa.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pby.wangshuangyany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://oom.yonumen.top

[I05] 按正则拆分
来源：http://xxn.zycfv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://byq.cashguo.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bhn.xuanzx.com

JS:   s.split(/\s*,\s*/)
来源：http://qza.jyoumei.cn

TS:   s.split(/\s*,\s*/)
来源：http://sdq.shanyushiyangtech.top

Java: s.split("\\s*,\\s*")
来源：http://ybu.ppjwa.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cxh.sysykeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://qzg.fzhhl.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ysz.hnxiangtu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dmr.yvedp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yox.guannengcc.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cyp.hcnkem.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kei.zdbjq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hhw.9152youxi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qjx.birdmap.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yls.guowangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ntq.jqgufenzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ewk.cucudq.cn

[I07] 忽略大小写与多行模式
来源：http://wrh.smart0.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ext.bjfxy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://odi.guannengcc.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zqs.zhiwuduotai.top

TS:   /error/gim
来源：http://fhl.feifeiyinyue.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://unv.epnwcf.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ddz.ehwqpu.com

Ruby: s.scan(/error/i)
来源：http://vfj.fehbvm.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rgd.zhiwuduotai.top

[I08] 贪婪与非贪婪匹配
来源：http://aop.yanxiufei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ysj.chenjidiqi.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://psz.birdmap.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hap.zhongyouzk.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://veg.hcnkem.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://zmw.aizwys.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://utz.feifeiyinyue.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ihg.smart0.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://njp.wangdashe.top

================================================================================
来源：http://jrk.daria6918.cn

J. 日期与时间
来源：http://nbt.nwbrower.top

================================================================================
来源：http://frd.daxiang520.top

[J01] 获取当前时间
来源：http://ewr.cucudq.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fuo.yongpay.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://etg.fktsv.cn

JS:   new Date();  Date.now()
来源：http://rch.hnxiangtu.top

TS:   new Date();  Date.now()
来源：http://krt.ydzc1.top

Java: LocalDateTime.now();  Instant.now()
来源：http://nvn.daria6918.cn

Go:   time.Now()
来源：http://szq.xuetiantiany.cn

Ruby: Time.now
来源：http://dqd.epnwcf.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://psz.jyoumei.cn

[J02] 格式化输出
来源：http://rch.uphjek.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cxs.ydjk.org.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vvu.wangdashe.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gkh.0kj1m.cn

TS:   d.toISOString()
来源：http://imt.andypj.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mlr.havefunace.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gtx.zhoulong.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xed.shzxlz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uwt.fehbvm.com

[J03] 字符串解析为日期
来源：http://bef.daria6918.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wwa.sxryk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://irl.uphjek.com

JS:   new Date("2024-01-02")
来源：http://zrv.yongpay.top

TS:   new Date("2024-01-02")
来源：http://lbr.chenlongwang.top

Java: LocalDate.parse("2024-01-02")
来源：http://vra.xuanzx.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pli.sufxvd.cn

Ruby: Date.parse("2024-01-02")
来源：http://afw.yanxiufei.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rem.yuanzhike.top

[J04] 时间戳与日期互转
来源：http://cex.zhijiandao.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pil.vqdsnc.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gxp.havefunace.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fvt.yongpay.top

TS:   Math.floor(Date.now() / 1000)
来源：http://kkm.yangfankeji.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nhx.uphjek.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mwu.hnqzz.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pkq.cashguo.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://aof.shangyingyoupin.top

[J05] 时间加减（加 7 天）
来源：http://jzi.yvedp.cn

Py:   now + timedelta(days=7)
来源：http://cix.xuetiantiany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bmk.9152youxi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cql.yanxiufei.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blf.shangyingyoupin.top

Java: LocalDate.now().plusDays(7)
来源：http://vwc.iojbl.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nbi.birdmap.top

Ruby: Time.now + 7 * 86400
来源：http://ctf.hfpthk.cn

C#:   DateTime.Now.AddDays(7)
来源：http://omt.cashguo.top

[J06] 计算两时间之差
来源：http://vtk.svipenyu.cn

Py:   (end - start).total_seconds()
来源：http://syz.yangfankeji.com

PHP:  $end->diff($start)->days;
来源：http://rvg.fengsongda.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qbl.bbcook.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wpc.jianghu66.top

Java: Duration.between(start, end).toSeconds()
来源：http://fdj.snrcjt.cn

Go:   end.Sub(start).Hours()
来源：http://vkf.ehwqpu.com

Ruby: end - start                 # 返回秒数
来源：http://nej.c1oappe.top

C#:   (end - start).TotalSeconds
来源：http://wvk.zhongyouzk.top

[J07] 比较两个日期
来源：http://xis.ctjpmb.com

Py:   d1 < d2;  d1 == d2
来源：http://jnp.daria6918.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://srf.nanxuanxn.top

JS:   d1.getTime() < d2.getTime()
来源：http://hey.quarkkingdee.top

TS:   d1.getTime() < d2.getTime()
来源：http://ryk.gotoacloud.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zqy.guowangkeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kto.havefunace.top

Ruby: d1 < d2;  d1 == d2
来源：http://zzq.yuanzhike.top

C#:   d1 < d2;  d1 == d2
来源：http://uco.cqqwz.cn

[J08] 提取年月日与星期
来源：http://mmf.cucudq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ylf.redwolf501.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://smy.shanyushiyangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://deb.yueranfly.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://csw.zhixingplan.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hfh.jinyuanbaomall.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bse.fehbvm.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tgl.vqdsnc.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ims.zhijiandao.cn

[J09] 时区处理
来源：http://gwh.xylfe.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gcv.aibaodan.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mgw.ivvv.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://noe.hnqzz.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jzg.feifeiyinyue.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lqt.hnqzz.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ecv.gogol.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xqa.pengpengdd.cyou

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tjf.fanxiaobao.xyz

[J10] 取今天 / 本月第一天
来源：http://yte.ctjpmb.com

Py:   date.today();  date.today().replace(day=1)
来源：http://lxg.tianlin.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bnp.ppjwa.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gay.aizwys.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oda.wangdashe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gos.pengpengdd.cyou

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nsr.zhixingplan.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tll.xylfe.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jmw.jyoumei.cn

================================================================================
来源：http://kqk.316326.xyz

K. JSON 与序列化
来源：http://usl.iojbl.cn

================================================================================
来源：http://isw.yonumen.top

[K01] 对象转 JSON 字符串
来源：http://mda.jqgfzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yka.ydjk.org.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jgj.ydzc1.top

JS:   JSON.stringify(obj)
来源：http://pdn.pycfn.com

TS:   JSON.stringify(obj)
来源：http://nqj.shzxlz.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nln.yangfankeji.com

Go:   json.Marshal(obj)
来源：http://tex.jqgfzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://dnp.pengpengdd.cyou

C#:   JsonSerializer.Serialize(obj)
来源：http://rlg.daxiang520.top

[K02] JSON 字符串转对象
来源：http://otw.jyoumei.cn

Py:   json.loads(s)
来源：http://mtz.xuanzx.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gfp.jinyuanbaomall.cn

JS:   JSON.parse(s)
来源：http://pnr.zhaomingkeji.xyz

TS:   JSON.parse(s)
来源：http://mjf.fanxiaobao.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lio.cashguo.top

Go:   json.Unmarshal(data, &v)
来源：http://miy.ppjwa.cn

Ruby: JSON.parse(s)
来源：http://zvw.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xzv.fehbvm.com

[K03] JSON 美化输出（带缩进）
来源：http://ppo.ydzc1.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xyf.cashguo.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wzh.pycfn.com

JS:   JSON.stringify(obj, null, 2)
来源：http://pbe.pengpengdd.cyou

TS:   JSON.stringify(obj, null, 2)
来源：http://aeh.quarkkingdee.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wch.nwbrower.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xvj.sufxvd.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ycc.fengsongda.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pyk.epnwcf.com

[K04] 读取 JSON 文件
来源：http://dgs.hongshengwenyu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://taz.jiagoushi.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yor.epnwcf.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yry.hongshengwenyu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eom.ywan-chungtsiang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qiw.fzhhl.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fmy.zycfv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tyt.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oiw.havefunace.top

[K05] 深拷贝对象
来源：http://bka.nanxuanxn.top

Py:   copy.deepcopy(obj)
来源：http://fhr.vqdsnc.cn

PHP:  unserialize(serialize($obj));
来源：http://zfy.9152youxi.cn

JS:   structuredClone(obj)
来源：http://gal.52xcode.cn

TS:   structuredClone(obj)
来源：http://jpf.jinghuilouyu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ast.jinyuanbaomall.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://deh.guannengcc.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bbq.gaohongyu789.top

C#:   // 序列化往返，或自定义 Clone
来源：http://nxw.fanxiaobao.xyz

[K06] 解析 URL 查询串
来源：http://aaw.gaohongyu789.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rfi.tian-w.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fvy.ivvv.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ese.hcnkem.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rmj.zhengqikj.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hke.gotoacloud.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ifh.xuanzx.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rkd.0kj1m.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pvj.xinyue.icu

[K07] 进制转换
来源：http://vcg.wangshuangyany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://klu.xylfe.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mmb.jinqigufen.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tqv.kuanghao11.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nhm.jiagoushi.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bya.guowangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mvg.cdnleiting.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://esb.uphjek.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iwn.sysykeji.top

[K08] 二进制序列化（非 JSON）
来源：http://gdt.dashuyun.cn

Py:   pickle.dumps(obj)
来源：http://uaq.sysykeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://foh.yj20258.top

JS:   v8.serialize(obj)        // Node
来源：http://ccc.tian-w.cn

TS:   v8.serialize(obj)        // Node
来源：http://xgi.ppjwa.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jtw.jlsjyb.cn

Go:   encoding/gob
来源：http://wyz.52xcode.cn

Ruby: Marshal.dump(obj)
来源：http://hjl.xinyue.icu

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rlw.yuanzhike.top

================================================================================
来源：http://efm.zhoulong.xyz

L. 网络请求
来源：http://zvf.yuanzhike.top

================================================================================
来源：http://zkg.daxiang520.top

[L01] 发送 GET 请求
来源：http://tys.sysykeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://atw.yonumen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rrr.zhengqikj.top

JS:   await fetch(url)
来源：http://tqr.dashuyun.cn

TS:   await fetch(url)
来源：http://qha.jianghu66.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://iah.aizwys.cn

Go:   resp, err := http.Get(url)
来源：http://ztd.cqqwz.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xld.uphjek.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mwh.jiagoushi.top

[L02] 发送 POST JSON
来源：http://jgs.yfazqb.com

Py:   requests.post(url, json={"a": 1})
来源：http://aic.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dow.hnqzz.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sqb.yangfankeji.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lkp.jinqigufen.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sqn.ywan-chungtsiang.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wxq.shangyingyoupin.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yfv.zhaomingkeji.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fmm.yj202588.top

[L03] 设置自定义请求头
来源：http://wom.sysykeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zsa.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bzf.pycfn.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vrb.ybcxt.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://icj.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://egj.hysaishi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hpe.gaohongyu789.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zzc.xuanzx.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nrn.xuetiantiany.cn

[L04] 设置超时
来源：http://vyz.xziqi.cn

Py:   requests.get(url, timeout=5)
来源：http://fwv.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ytr.iojbl.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://civ.nanxinkj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fpz.xziqi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://brf.yanxiufei.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qxt.guannengcc.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://osn.aibaodan.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wrp.wangdashe.top

[L05] 上传文件（multipart）
来源：http://qfq.snrcjt.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fdr.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rge.meibo888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lta.cdnleiting.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kes.chenjidiqi.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nsb.316326.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hpc.svipenyu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nho.vqdsnc.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ccv.ctjpmb.com

[L06] 解析响应为 JSON
来源：http://ajo.yj202588.top

Py:   resp.json()
来源：http://zcz.zdqjudy.top

PHP:  json_decode($body, true);
来源：http://zei.shanyushiyangtech.top

JS:   await resp.json()
来源：http://nny.cashguo.top

TS:   await resp.json()
来源：http://mrs.hesvh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ggb.zdbjq.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ndf.jinqigufen.top

Ruby: JSON.parse(resp.body)
来源：http://xaq.wangdashe.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dgs.yueranfly.top

[L07] 处理 HTTP 状态码
来源：http://szj.hywenlv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://iof.zhoulong.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ysr.hnxiangtu.top

JS:   resp.ok;  resp.status
来源：http://tiy.bbcook.cn

TS:   resp.ok;  resp.status
来源：http://ktu.jinqigufen.top

Java: resp.statusCode()
来源：http://tuj.birdmap.top

Go:   resp.StatusCode
来源：http://oon.dashuyun.cn

Ruby: resp.code.to_i
来源：http://zek.yvedp.cn

C#:   (int)resp.StatusCode
来源：http://zuw.chenlongwang.top

[L08] 并发请求多个地址
来源：http://ijy.chenlongwang.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hus.tanke756.top

PHP:  curl_multi_init() 系列
来源：http://fex.zdqjudy.top


<!-- 参考信息 -->