代发 wailian999

TS:   s.match(/\d+/g)
来源：http://kqc.fktsv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kdx.hcnkem.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bjm.xuetiantiany.cn

Ruby: s.scan(/\d+/)
来源：http://raq.hysaishi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ojv.316326.xyz

[I03] 提取捕获分组
来源：http://wck.fzhhl.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sxq.havefunace.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tcl.0kj1m.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pxr.tarul.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://moi.pengpengdd.cyou

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://opt.svipenyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://udq.cqqwz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hbf.gogol.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dae.fanxiaobao.xyz

[I04] 正则替换
来源：http://gyl.zhijiandao.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ump.jinghuilouyu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tiy.yueranfly.top

JS:   s.replace(/\d+/g, "#")
来源：http://yjd.yj202588.top

TS:   s.replace(/\d+/g, "#")
来源：http://ofa.zdqjudy.top

Java: s.replaceAll("\\d+", "#")
来源：http://rzf.pycfn.com

Go:   re.ReplaceAllString(s, "#")
来源：http://xbx.shangyingyoupin.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nha.uphjek.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dfc.daria6918.cn

[I05] 按正则拆分
来源：http://nfd.shangyingyoupin.top

Py:   re.split(r"\s*,\s*", s)
来源：http://mwd.yj20258888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cyj.chenjidiqi.icu

JS:   s.split(/\s*,\s*/)
来源：http://vkq.jinyuanbaomall.cn

TS:   s.split(/\s*,\s*/)
来源：http://dxz.mhx1999.top

Java: s.split("\\s*,\\s*")
来源：http://kpd.zycfv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vxl.jinqigufen.top

Ruby: s.split(/\s*,\s*/)
来源：http://ewo.jiagoushi.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rya.ydzc1.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://esj.snrcjt.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ntg.yuanzhike.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gik.dianchejie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ewx.daria6918.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://duf.aizwys.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://teu.zycfv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fet.c1oappe.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://olh.cqqwz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oea.jqgufenzy.top

[I07] 忽略大小写与多行模式
来源：http://nma.hcnkem.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wkf.xuanzx.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fbn.xinyue.icu

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ngb.ctjpmb.com

TS:   /error/gim
来源：http://aep.aibaodan.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mdc.jinqigufen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fng.yuanzhike.top

Ruby: s.scan(/error/i)
来源：http://rel.jianghu66.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://edf.sysykeji.top

[I08] 贪婪与非贪婪匹配
来源：http://fxk.fanxiaobao.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vis.iojbl.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://aix.jinqigufen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lwq.gaohongyu789.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://juc.ydjk.org.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ehn.cdnleiting.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://svu.xziqi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yxc.meibo888.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lic.shzxlz.cn

================================================================================
来源：http://mmm.gaohongyu789.top

J. 日期与时间
来源：http://qrf.tian-w.cn

================================================================================
来源：http://ygo.wangshuangyany.cn

[J01] 获取当前时间
来源：http://fql.hesvh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pbh.jinghuilouyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ess.tarul.cn

JS:   new Date();  Date.now()
来源：http://lwx.aizwys.cn

TS:   new Date();  Date.now()
来源：http://ftw.ydzc1.top

Java: LocalDateTime.now();  Instant.now()
来源：http://kcn.kuanghao11.cn

Go:   time.Now()
来源：http://opp.pengpengdd.cyou

Ruby: Time.now
来源：http://hhs.yuanzhike.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tdq.hcnkem.com

[J02] 格式化输出
来源：http://xso.fanxiaobao.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dwp.tian-w.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cja.hnqzz.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://swo.hysaishi.cn

TS:   d.toISOString()
来源：http://vqc.shanyushiyangtech.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rql.zhijiandao.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pxm.yuxming.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fom.hywenlv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cnq.andypj.xyz

[J03] 字符串解析为日期
来源：http://krf.fktsv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fbd.yuxming.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kcw.haohaochexian.top

JS:   new Date("2024-01-02")
来源：http://xuo.sweek.top

TS:   new Date("2024-01-02")
来源：http://mqk.gaohongyu789.top

Java: LocalDate.parse("2024-01-02")
来源：http://ruz.jinqigfzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tef.mhx1999.top

Ruby: Date.parse("2024-01-02")
来源：http://eoz.ctjpmb.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oro.fengsongda.top

[J04] 时间戳与日期互转
来源：http://zqf.nanxinkj.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nge.snrcjt.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ndv.jinqigufen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dva.yvedp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zfo.ywan-chungtsiang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ewn.cashguo.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ryj.ybcxt.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dba.sxryk.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pqc.chenlongwang.top

[J05] 时间加减（加 7 天）
来源：http://ftw.xziqi.cn

Py:   now + timedelta(days=7)
来源：http://ncd.hfpthk.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://isv.nwbrower.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lug.snrcjt.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://juj.aizwys.cn

Java: LocalDate.now().plusDays(7)
来源：http://ukr.fktsv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zfj.gotoacloud.top

Ruby: Time.now + 7 * 86400
来源：http://ngd.tanke756.top

C#:   DateTime.Now.AddDays(7)
来源：http://nml.jqgfzy.top

[J06] 计算两时间之差
来源：http://ruj.nanxuanxn.top

Py:   (end - start).total_seconds()
来源：http://zum.jlsjyb.cn

PHP:  $end->diff($start)->days;
来源：http://gbl.ctjpmb.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://azt.mhx1999.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kvd.sweek.top

Java: Duration.between(start, end).toSeconds()
来源：http://sak.zycfv.cn

Go:   end.Sub(start).Hours()
来源：http://xda.aizwys.cn

Ruby: end - start                 # 返回秒数
来源：http://nza.dianchejie.cn

C#:   (end - start).TotalSeconds
来源：http://xwk.iojbl.cn

[J07] 比较两个日期
来源：http://xus.tian-w.cn

Py:   d1 < d2;  d1 == d2
来源：http://jjj.jlsjyb.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ant.yfazqb.com

JS:   d1.getTime() < d2.getTime()
来源：http://liw.meibo888.top

TS:   d1.getTime() < d2.getTime()
来源：http://kky.ehwqpu.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yug.yfazqb.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vic.zhiwuduotai.top

Ruby: d1 < d2;  d1 == d2
来源：http://jsr.vqdsnc.cn

C#:   d1 < d2;  d1 == d2
来源：http://doq.sysykeji.top

[J08] 提取年月日与星期
来源：http://tof.chenlongwang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lfn.shanyushiyangtech.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://smd.hfpthk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nhv.shangyingyoupin.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pdz.0kj1m.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tvu.ybcxt.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fms.fehbvm.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ocy.ydjk.org.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ayl.shzxlz.cn

[J09] 时区处理
来源：http://dia.hcnkem.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fkf.chenjidiqi.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qph.nanxinkj.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qty.dianchejie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wgu.fzhhl.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uhi.9152youxi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rud.zhixingplan.top

Ruby: Time.now.getlocal("+08:00")
来源：http://jyg.fzhhl.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://syo.svipenyu.cn

[J10] 取今天 / 本月第一天
来源：http://bys.fengsongda.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rke.52xcode.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mbk.ybcxt.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://osg.zhiwuduotai.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://puj.bbcook.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rsq.dashuyun.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kdq.yj20258.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wmp.tanke756.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jxs.52xcode.cn

================================================================================
来源：http://fbk.dianchejie.cn

K. JSON 与序列化
来源：http://xob.jqgufenzy.top

================================================================================
来源：http://jde.chenzaomai.com

[K01] 对象转 JSON 字符串
来源：http://tjs.zhengqikj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kmm.ctjpmb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dzv.nanxinkj.top

JS:   JSON.stringify(obj)
来源：http://igl.hywenlv.cn

TS:   JSON.stringify(obj)
来源：http://wrd.ivvv.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rfz.fengsongda.top

Go:   json.Marshal(obj)
来源：http://mfq.svipenyu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nod.ydzc1.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qtf.jqgufenzy.top

[K02] JSON 字符串转对象
来源：http://eez.ydzc1.top

Py:   json.loads(s)
来源：http://vxv.meibo888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ymp.zdbjq.cn

JS:   JSON.parse(s)
来源：http://yhx.redwolf501.top

TS:   JSON.parse(s)
来源：http://vvw.tanke756.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tkn.bbcook.cn

Go:   json.Unmarshal(data, &v)
来源：http://xdp.jlsjyb.cn

Ruby: JSON.parse(s)
来源：http://soc.zhixingplan.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fqv.ctjpmb.com

[K03] JSON 美化输出（带缩进）
来源：http://sbb.nanxuanxn.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lam.pengpengdd.cyou

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ppm.hywenlv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dlt.ydzc1.top

TS:   JSON.stringify(obj, null, 2)
来源：http://akb.shzxlz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yhp.dianchejie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fax.snrcjt.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fhi.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://imb.zhaomingkeji.xyz

[K04] 读取 JSON 文件
来源：http://ekm.jianghu66.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cco.hnxiangtu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://etf.feifeiyinyue.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hrx.guowangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nbm.xylfe.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qpo.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kev.dashuyun.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jqa.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jif.guowangkeji.top

[K05] 深拷贝对象
来源：http://dnr.aizwys.cn

Py:   copy.deepcopy(obj)
来源：http://tay.gaohongyu789.top

PHP:  unserialize(serialize($obj));
来源：http://ewp.redwolf501.top

JS:   structuredClone(obj)
来源：http://tmd.meibo888.top

TS:   structuredClone(obj)
来源：http://dwz.mhx1999.top

Java: // 手写拷贝构造，或序列化往返
来源：http://rqo.aizwys.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pon.shangyingyoupin.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://goy.kuanghao11.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://eyw.kuanghao11.cn

[K06] 解析 URL 查询串
来源：http://hhu.chenlongwang.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ztn.ivvv.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fsu.sufxvd.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://coz.yfazqb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://opm.jinqigufen.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zhe.bbcook.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fum.uphjek.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gsc.zdbjq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dzw.yuanzhike.top

[K07] 进制转换
来源：http://ogh.yj20258888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jvq.guowangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dsu.snrcjt.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kuj.cashguo.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dkv.ehwqpu.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cwh.jiagoushi.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://snf.0kj1m.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ovq.yj20258.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fgv.uphjek.com

[K08] 二进制序列化（非 JSON）
来源：http://kqw.mhx1999.top

Py:   pickle.dumps(obj)
来源：http://erh.yueranfly.top

PHP:  serialize($obj);  unserialize($s);
来源：http://siv.vqdsnc.cn

JS:   v8.serialize(obj)        // Node
来源：http://czc.hcnkem.com

TS:   v8.serialize(obj)        // Node
来源：http://dem.yuxming.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fxf.hnxiangtu.top

Go:   encoding/gob
来源：http://lsl.haohaochexian.top

Ruby: Marshal.dump(obj)
来源：http://tnh.fehbvm.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://idm.shangyingyoupin.top

================================================================================
来源：http://ayg.fehbvm.com

L. 网络请求
来源：http://gdt.pycfn.com

================================================================================
来源：http://djh.zhaomingkeji.xyz

[L01] 发送 GET 请求
来源：http://osj.jinyuanbaomall.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cpj.hongshengwenyu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vcm.sysykeji.top

JS:   await fetch(url)
来源：http://sia.yanxiufei.cn

TS:   await fetch(url)
来源：http://lib.fzhhl.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ljv.mhx1999.top

Go:   resp, err := http.Get(url)
来源：http://jyf.uphjek.com

Ruby: Net::HTTP.get(URI(url))
来源：http://hgp.kuanghao11.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://src.tian-w.cn

[L02] 发送 POST JSON
来源：http://ubh.sjlbkw.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jfl.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nbt.yangfankeji.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://apn.gotoacloud.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sgx.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qys.jyoumei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gxc.cashguo.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://agc.zycfv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pvw.ivvv.top

[L03] 设置自定义请求头
来源：http://gnn.tanke756.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ppe.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jif.zhengqikj.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rop.quarkkingdee.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hqu.havefunace.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lro.nwbrower.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iot.hesvh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qcc.ydjk.org.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mtz.redwolf501.top

[L04] 设置超时
来源：http://rki.redwolf501.top

Py:   requests.get(url, timeout=5)
来源：http://jdu.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pjq.dashuyun.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ebm.vqdsnc.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vvq.xuetiantiany.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yul.jinqigfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lke.gogol.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jzw.ctjpmb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gyc.hfpthk.cn

[L05] 上传文件（multipart）
来源：http://jge.sjlbkw.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zbn.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://epm.ydjk.org.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://epf.jinqigfzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gkg.haohaochexian.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gqb.daria6918.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ndy.yanxiufei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rdh.pengpengdd.cyou

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ati.yj20258888.top

[L06] 解析响应为 JSON
来源：http://bou.svipenyu.cn

Py:   resp.json()
来源：http://gly.jqgfzy.top

PHP:  json_decode($body, true);
来源：http://pmk.yanxiufei.cn

JS:   await resp.json()
来源：http://xgy.gzhubu.top

TS:   await resp.json()
来源：http://xzk.daria6918.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kzs.pycfn.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hpx.iojbl.cn

Ruby: JSON.parse(resp.body)
来源：http://yaq.havefunace.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bqx.tanke756.top

[L07] 处理 HTTP 状态码
来源：http://yhv.bbcook.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kzx.cheryme.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jhl.zhongyouzk.top

JS:   resp.ok;  resp.status
来源：http://pqq.yueranfly.top

TS:   resp.ok;  resp.status
来源：http://xue.kuanghao11.cn

Java: resp.statusCode()
来源：http://fbm.svipenyu.cn

Go:   resp.StatusCode
来源：http://qmj.sxryk.cn

Ruby: resp.code.to_i
来源：http://vrk.zhongyouzk.top

C#:   (int)resp.StatusCode
来源：http://jzv.iojbl.cn

[L08] 并发请求多个地址
来源：http://ugn.ppjwa.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yut.jqgfzy.top

PHP:  curl_multi_init() 系列
来源：http://awx.yangfankeji.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://akm.fanxiaobao.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gnc.jinyuanbaomall.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gwu.uphjek.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uxg.gogol.net.cn


<!-- 参考信息 -->