代发 wailian999

[I02] 提取所有匹配
来源：http://yea.bbcook.cn

Py:   re.findall(r"\d+", s)
来源：http://tzb.birdmap.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gud.havefunace.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mbn.ehwqpu.com

TS:   s.match(/\d+/g)
来源：http://bqz.chenzaomai.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sit.hcnkem.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cso.gzhubu.top

Ruby: s.scan(/\d+/)
来源：http://mtu.jqgufenzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ysz.hysaishi.cn

[I03] 提取捕获分组
来源：http://gcw.kuanghao11.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://itg.xuetiantiany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tfg.ivvv.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fms.xuetiantiany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ahr.yuxming.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qey.wangshuangyany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nys.fehbvm.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wlp.cqqwz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vlu.svipenyu.cn

[I04] 正则替换
来源：http://ufb.c1oappe.top

Py:   re.sub(r"\d+", "#", s)
来源：http://izf.zhiwuduotai.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ypz.guannengcc.top

JS:   s.replace(/\d+/g, "#")
来源：http://vcr.nanxinkj.top

TS:   s.replace(/\d+/g, "#")
来源：http://phh.yongpay.top

Java: s.replaceAll("\\d+", "#")
来源：http://czt.zhiwuduotai.top

Go:   re.ReplaceAllString(s, "#")
来源：http://osb.hysaishi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ndt.fanxiaobao.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nlc.cashguo.top

[I05] 按正则拆分
来源：http://rpm.9152youxi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wqq.hongshengwenyu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bxn.jqgfzy.top

JS:   s.split(/\s*,\s*/)
来源：http://eab.yanxiufei.cn

TS:   s.split(/\s*,\s*/)
来源：http://gdi.sufxvd.cn

Java: s.split("\\s*,\\s*")
来源：http://sev.chenlongwang.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bek.guowangkeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://uar.tian-w.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ahw.shanyushiyangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nop.fengsongda.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dro.nwbrower.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fsk.yonumen.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eci.jinqigfzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dsk.ybcxt.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zrr.316326.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://guf.shanyushiyangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://aya.dashuyun.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tbi.xuanzx.com

[I07] 忽略大小写与多行模式
来源：http://xzl.birdmap.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wdg.fengsongda.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oif.mhx1999.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ucg.hongshengwenyu.top

TS:   /error/gim
来源：http://tuo.snrcjt.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oqu.dashuyun.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wpn.jiagoushi.top

Ruby: s.scan(/error/i)
来源：http://htx.wangdashe.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://acj.yongpay.top

[I08] 贪婪与非贪婪匹配
来源：http://ppf.tarul.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vla.xuanzx.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://unh.chenlongwang.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kjj.zhiwuduotai.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mxg.guowangkeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://vzn.cucudq.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eso.yonumen.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://apr.ywan-chungtsiang.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zga.sjlbkw.cn

================================================================================
来源：http://ghi.ehwqpu.com

J. 日期与时间
来源：http://pbj.pycfn.com

================================================================================
来源：http://ezz.yuanzhike.top

[J01] 获取当前时间
来源：http://wnb.shanyushiyangtech.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jjm.yj202588.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sat.zycfv.cn

JS:   new Date();  Date.now()
来源：http://nwx.pengpengdd.cyou

TS:   new Date();  Date.now()
来源：http://uhx.ppjwa.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bno.nanxuanxn.top

Go:   time.Now()
来源：http://xgr.yvedp.cn

Ruby: Time.now
来源：http://mbw.hywenlv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tif.yongpay.top

[J02] 格式化输出
来源：http://cvu.fktsv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nvd.redwolf501.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jin.hammf.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://itc.tian-w.cn

TS:   d.toISOString()
来源：http://rja.yj20258888.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sha.wangshuangyany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nzo.yuxming.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jih.hesvh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lty.bbcook.cn

[J03] 字符串解析为日期
来源：http://jzk.yuanzhike.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gkz.shzxlz.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fei.ydzc1.top

JS:   new Date("2024-01-02")
来源：http://goi.chenjidiqi.icu

TS:   new Date("2024-01-02")
来源：http://xzz.zhiwuduotai.top

Java: LocalDate.parse("2024-01-02")
来源：http://nen.ybcxt.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fxm.shzxlz.cn

Ruby: Date.parse("2024-01-02")
来源：http://hvf.0kj1m.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lzp.kuanghao11.cn

[J04] 时间戳与日期互转
来源：http://zzh.ywan-chungtsiang.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hyx.hongshengwenyu.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sfj.chenlongwang.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rhh.havefunace.top

TS:   Math.floor(Date.now() / 1000)
来源：http://iih.hammf.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yzz.hfpthk.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yvf.yueranfly.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zky.dianchejie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://elz.hnxiangtu.top

[J05] 时间加减（加 7 天）
来源：http://huo.zycfv.cn

Py:   now + timedelta(days=7)
来源：http://ioy.cheryme.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://noc.zhixingplan.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mpm.ppjwa.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qvv.sysykeji.top

Java: LocalDate.now().plusDays(7)
来源：http://kmp.shanyushiyangkeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uhp.shzxlz.cn

Ruby: Time.now + 7 * 86400
来源：http://qwc.jlsjyb.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fzg.sxryk.cn

[J06] 计算两时间之差
来源：http://pyp.zhengqikj.top

Py:   (end - start).total_seconds()
来源：http://rup.haohaochexian.top

PHP:  $end->diff($start)->days;
来源：http://kqe.shanyushiyangtech.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://omi.xuanzx.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jfq.aibaodan.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kry.52xcode.cn

Go:   end.Sub(start).Hours()
来源：http://ihx.feifeiyinyue.top

Ruby: end - start                 # 返回秒数
来源：http://ygn.iojbl.cn

C#:   (end - start).TotalSeconds
来源：http://zha.c1oappe.top

[J07] 比较两个日期
来源：http://bfm.fanxiaobao.xyz

Py:   d1 < d2;  d1 == d2
来源：http://rxk.mhx1999.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pvv.yangfankeji.com

JS:   d1.getTime() < d2.getTime()
来源：http://vzx.sjlbkw.cn

TS:   d1.getTime() < d2.getTime()
来源：http://izo.yangfankeji.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://agz.ppjwa.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hzf.cheryme.top

Ruby: d1 < d2;  d1 == d2
来源：http://hga.cdnleiting.top

C#:   d1 < d2;  d1 == d2
来源：http://xhp.jiagoushi.top

[J08] 提取年月日与星期
来源：http://hmi.ywan-chungtsiang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bxs.gzhubu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hia.aizwys.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nkf.jiagoushi.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nxk.havefunace.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ggt.hammf.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fap.fzhhl.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hmu.hnxiangtu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xrj.ywan-chungtsiang.top

[J09] 时区处理
来源：http://rcn.vqdsnc.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rbk.ydjk.org.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xds.kuanghao11.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bdh.yuanzhike.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://toa.nwbrower.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xor.shangyingyoupin.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qqe.jinghuilouyu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://heb.jqgufenzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ghz.jqgfzy.top

[J10] 取今天 / 本月第一天
来源：http://fpk.ydjk.org.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://sci.yuxming.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://swi.gotoacloud.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vom.vehdjk.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://juj.sweek.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lmf.xinyue.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bvb.fanxiaobao.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ewv.tianlin.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ucp.kuanghao11.cn

================================================================================
来源：http://dwl.sysykeji.top

K. JSON 与序列化
来源：http://ydu.fehbvm.com

================================================================================
来源：http://akn.c1oappe.top

[K01] 对象转 JSON 字符串
来源：http://gpz.yuanzhike.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rjv.jinghuilouyu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rgw.zhengqikj.top

JS:   JSON.stringify(obj)
来源：http://kfk.sysykeji.top

TS:   JSON.stringify(obj)
来源：http://yon.tianlin.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lin.guannengcc.top

Go:   json.Marshal(obj)
来源：http://yat.mhx1999.top

Ruby: obj.to_json                                     // require "json"
来源：http://abq.yj20258.top

C#:   JsonSerializer.Serialize(obj)
来源：http://sri.hesvh.cn

[K02] JSON 字符串转对象
来源：http://srm.ywan-chungtsiang.top

Py:   json.loads(s)
来源：http://oer.yangfankeji.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ycz.sufxvd.cn

JS:   JSON.parse(s)
来源：http://syv.gzhubu.top

TS:   JSON.parse(s)
来源：http://smp.ehwqpu.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ufo.yongpay.top

Go:   json.Unmarshal(data, &v)
来源：http://yyy.cucudq.cn

Ruby: JSON.parse(s)
来源：http://tnd.uphjek.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dad.zhongyouzk.top

[K03] JSON 美化输出（带缩进）
来源：http://hgl.daxiang520.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://adh.zhongyouzk.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vid.zhengqikj.top

JS:   JSON.stringify(obj, null, 2)
来源：http://lut.yfazqb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://shu.shangyingyoupin.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xoj.guowangkeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://naa.yj20258.top

Ruby: JSON.pretty_generate(obj)
来源：http://pgc.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bju.yonumen.top

[K04] 读取 JSON 文件
来源：http://fcn.guowangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mpr.daria6918.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://odu.pengpengdd.cyou

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://drq.mhx1999.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://odl.cqqwz.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jqb.yj202588.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vxd.fanxiaobao.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://ayl.andypj.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fwf.ydzc1.top

[K05] 深拷贝对象
来源：http://oyr.zycfv.cn

Py:   copy.deepcopy(obj)
来源：http://kgn.jinqigfzy.top

PHP:  unserialize(serialize($obj));
来源：http://kme.mhx1999.top

JS:   structuredClone(obj)
来源：http://ecs.sxryk.cn

TS:   structuredClone(obj)
来源：http://ksp.gzhubu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://woj.zdqjudy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jer.tianlin.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zts.gogol.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hsa.shanyushiyangtech.top

[K06] 解析 URL 查询串
来源：http://jqa.ywan-chungtsiang.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://evr.xingfuxueyuan.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://srr.quarkkingdee.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cvo.snrcjt.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ghz.pycfn.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://luc.xinyue.icu

Go:   url.ParseQuery("a=1&b=2")
来源：http://cxc.yuxming.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qpr.guowangkeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mim.fktsv.cn

[K07] 进制转换
来源：http://qib.vqdsnc.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hlt.svipenyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lcm.ppjwa.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://edg.snrcjt.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nca.guowangkeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rpn.smart0.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qdv.jiagoushi.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zjo.zhengqikj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://okc.aizwys.cn

[K08] 二进制序列化（非 JSON）
来源：http://jnu.guowangkeji.top

Py:   pickle.dumps(obj)
来源：http://lsp.9152youxi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://loa.quarkkingdee.top

JS:   v8.serialize(obj)        // Node
来源：http://box.yj20258.top

TS:   v8.serialize(obj)        // Node
来源：http://kyw.sufxvd.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dle.tanke756.top

Go:   encoding/gob
来源：http://tbn.redwolf501.top

Ruby: Marshal.dump(obj)
来源：http://rac.mhx1999.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lkt.ctjpmb.com

================================================================================
来源：http://mqd.ppjwa.cn

L. 网络请求
来源：http://fpw.nanxinkj.top

================================================================================
来源：http://hhv.bbcook.cn

[L01] 发送 GET 请求
来源：http://cdg.gotoacloud.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dsv.yonumen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://caw.ivvv.top

JS:   await fetch(url)
来源：http://irc.52xcode.cn

TS:   await fetch(url)
来源：http://hdn.cashguo.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://llu.uphjek.com

Go:   resp, err := http.Get(url)
来源：http://wdk.sweek.top

Ruby: Net::HTTP.get(URI(url))
来源：http://guh.52xcode.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://clu.ybcxt.top

[L02] 发送 POST JSON
来源：http://rru.chenjidiqi.icu

Py:   requests.post(url, json={"a": 1})
来源：http://vzu.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yhq.yuxming.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ulv.ybcxt.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vve.yfazqb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sta.zhiwuduotai.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hxm.chenjidiqi.icu

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yhr.shzxlz.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sgk.shangyingyoupin.top

[L03] 设置自定义请求头
来源：http://jul.gotoacloud.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zoi.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://djl.jqgufenzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tas.shangyingyoupin.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lpt.hesvh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ois.meibo888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xpf.jqgfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bvt.daria6918.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ibi.zhongyouzk.top

[L04] 设置超时
来源：http://qei.hfpthk.cn

Py:   requests.get(url, timeout=5)
来源：http://kcs.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gpb.mhx1999.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bie.gaohongyu789.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aso.uphjek.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hdl.aibaodan.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dft.snrcjt.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://luu.mhx1999.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uwz.nanxuanxn.top

[L05] 上传文件（multipart）
来源：http://ccb.sxryk.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rgm.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vyn.c1oappe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gsz.iojbl.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qiv.chenjidiqi.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mzd.zhaomingkeji.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kcm.kuanghao11.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dqz.aizwys.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kvs.zhiwuduotai.top

[L06] 解析响应为 JSON
来源：http://upc.guannengcc.top

Py:   resp.json()
来源：http://nnw.9152youxi.cn

PHP:  json_decode($body, true);
来源：http://xpv.shanyushiyangtech.top

JS:   await resp.json()
来源：http://xkd.zdqjudy.top

TS:   await resp.json()
来源：http://vbw.sxryk.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gwd.zdqjudy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jca.hnqzz.top

Ruby: JSON.parse(resp.body)
来源：http://amj.fanxiaobao.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hxa.gogol.net.cn

[L07] 处理 HTTP 状态码
来源：http://yqr.hnxiangtu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qyv.dianchejie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ora.jinqigfzy.top

JS:   resp.ok;  resp.status
来源：http://hdd.birdmap.top

TS:   resp.ok;  resp.status
来源：http://wln.shangyingyoupin.top

Java: resp.statusCode()
来源：http://zko.jinyuanbaomall.cn

Go:   resp.StatusCode
来源：http://xar.meibo888.top

Ruby: resp.code.to_i
来源：http://ase.jinyuanbaomall.cn

C#:   (int)resp.StatusCode
来源：http://sir.uphjek.com

[L08] 并发请求多个地址
来源：http://cux.epnwcf.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pxc.zhijiandao.cn

PHP:  curl_multi_init() 系列
来源：http://xrp.daxiang520.top


<!-- 参考信息 -->