代发 wailian999

TS:   s.match(/\d+/g)
来源：http://ooj.0kj1m.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://say.wangdashe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kjv.jqgufenzy.top

Ruby: s.scan(/\d+/)
来源：http://icc.hnqzz.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bvm.yanxiufei.cn

[I03] 提取捕获分组
来源：http://qqs.pycfn.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kpd.yuanzhike.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://och.sysykeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lvp.jqgufenzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vqs.jinghuilouyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qrf.redwolf501.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ywv.zdbjq.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://daw.jiagoushi.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lnh.ydzc1.top

[I04] 正则替换
来源：http://ogd.bjfxy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ujg.xylfe.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pva.sysykeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://biv.cdnleiting.top

TS:   s.replace(/\d+/g, "#")
来源：http://trk.hnxiangtu.top

Java: s.replaceAll("\\d+", "#")
来源：http://nkq.vehdjk.com

Go:   re.ReplaceAllString(s, "#")
来源：http://kcw.daria6918.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://aom.cheryme.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://iii.chenzaomai.com

[I05] 按正则拆分
来源：http://vuf.andypj.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://lzh.snrcjt.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bul.zhaomingkeji.xyz

JS:   s.split(/\s*,\s*/)
来源：http://iqw.sysykeji.top

TS:   s.split(/\s*,\s*/)
来源：http://ijn.birdmap.top

Java: s.split("\\s*,\\s*")
来源：http://eeg.wangdashe.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qhx.hnqzz.top

Ruby: s.split(/\s*,\s*/)
来源：http://sut.aibaodan.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qno.shanyushiyangtech.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jam.hcnkem.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gzl.ybcxt.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://asp.xingfuxueyuan.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jjx.fzhhl.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cdo.ydjk.org.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qrv.fehbvm.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://czt.hfpthk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lzx.yongpay.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pty.guowangkeji.top

[I07] 忽略大小写与多行模式
来源：http://lwr.vqdsnc.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xnz.hcnkem.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vmq.snrcjt.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sdd.yvedp.cn

TS:   /error/gim
来源：http://qrl.nwbrower.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yvz.ppjwa.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vbh.svipenyu.cn

Ruby: s.scan(/error/i)
来源：http://kkk.zycfv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pcy.feifeiyinyue.top

[I08] 贪婪与非贪婪匹配
来源：http://eva.cqqwz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vbd.fehbvm.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tvz.ppjwa.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gil.0kj1m.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kzl.quarkkingdee.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qkw.zhongyouzk.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eme.cqqwz.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lse.cdnleiting.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://eht.hcnkem.com

================================================================================
来源：http://cji.shanyushiyangtech.top

J. 日期与时间
来源：http://vai.fanxiaobao.xyz

================================================================================
来源：http://trv.xuanzx.com

[J01] 获取当前时间
来源：http://ymp.zycfv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yog.jinqigufen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bjm.yanxiufei.cn

JS:   new Date();  Date.now()
来源：http://zqq.xylfe.cn

TS:   new Date();  Date.now()
来源：http://xvq.ppjwa.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rsg.daria6918.cn

Go:   time.Now()
来源：http://abz.ivvv.top

Ruby: Time.now
来源：http://wro.jinghuilouyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://syi.tanke756.top

[J02] 格式化输出
来源：http://zcj.chenlongwang.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ran.pengpengdd.cyou

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dsh.xingfuxueyuan.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bws.fanxiaobao.xyz

TS:   d.toISOString()
来源：http://ezr.bbcook.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ots.dashuyun.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xtt.shanyushiyangtech.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gun.yj20258888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cak.fengsongda.top

[J03] 字符串解析为日期
来源：http://vxz.vehdjk.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fel.cucudq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wql.shzxlz.cn

JS:   new Date("2024-01-02")
来源：http://ksl.dianchejie.cn

TS:   new Date("2024-01-02")
来源：http://avk.tian-w.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hoe.jianghu66.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yee.yfazqb.com

Ruby: Date.parse("2024-01-02")
来源：http://rke.ydjk.org.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xeg.uphjek.com

[J04] 时间戳与日期互转
来源：http://cme.tian-w.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cqr.zycfv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cwj.wangdashe.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wfc.xylfe.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wns.gaohongyu789.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wmm.cdnleiting.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sob.cheryme.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zel.aizwys.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qwg.hysaishi.cn

[J05] 时间加减（加 7 天）
来源：http://gid.yj202588.top

Py:   now + timedelta(days=7)
来源：http://fyp.bbcook.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tov.yfazqb.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cne.jlsjyb.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uyt.jinqigfzy.top

Java: LocalDate.now().plusDays(7)
来源：http://mrr.yj202588.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fxc.redwolf501.top

Ruby: Time.now + 7 * 86400
来源：http://mbh.fanxiaobao.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://slw.zhijiandao.cn

[J06] 计算两时间之差
来源：http://fwl.bjfxy.top

Py:   (end - start).total_seconds()
来源：http://ftp.ctjpmb.com

PHP:  $end->diff($start)->days;
来源：http://svo.ydjk.org.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://krv.yangfankeji.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uph.yj20258888.top

Java: Duration.between(start, end).toSeconds()
来源：http://gwl.zycfv.cn

Go:   end.Sub(start).Hours()
来源：http://ajy.birdmap.top

Ruby: end - start                 # 返回秒数
来源：http://gjb.cheryme.top

C#:   (end - start).TotalSeconds
来源：http://las.redwolf501.top

[J07] 比较两个日期
来源：http://sov.yj20258888.top

Py:   d1 < d2;  d1 == d2
来源：http://cgg.chenjidiqi.icu

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://psn.yfazqb.com

JS:   d1.getTime() < d2.getTime()
来源：http://qii.guannengcc.top

TS:   d1.getTime() < d2.getTime()
来源：http://uom.tianlin.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wrr.hfpthk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hgu.vqdsnc.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qhg.fengsongda.top

C#:   d1 < d2;  d1 == d2
来源：http://eyo.jinqigfzy.top

[J08] 提取年月日与星期
来源：http://kkx.jinyuanbaomall.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uok.wangdashe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dcn.jinqigfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://crr.shanyushiyangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xts.jlsjyb.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gye.gzhubu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gcp.dianchejie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://udq.zhijiandao.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ygm.jiagoushi.top

[J09] 时区处理
来源：http://ucd.nwbrower.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xho.cdnleiting.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hfe.jianghu66.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ufv.daria6918.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://abh.chenlongwang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://etj.52xcode.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wfi.jinqigfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://oya.sxryk.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://urf.chenzaomai.com

[J10] 取今天 / 本月第一天
来源：http://wjy.haohaochexian.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rsa.zycfv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://crt.yongpay.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://imh.meibo888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pib.yj20258888.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wiu.xziqi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dry.tarul.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cyv.zhongyouzk.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wha.haohaochexian.top

================================================================================
来源：http://sym.jiagoushi.top

K. JSON 与序列化
来源：http://kjn.guowangkeji.top

================================================================================
来源：http://rpu.nanxuanxn.top

[K01] 对象转 JSON 字符串
来源：http://mmh.daxiang520.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fga.yj20258.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://krh.9152youxi.cn

JS:   JSON.stringify(obj)
来源：http://erq.ivvv.top

TS:   JSON.stringify(obj)
来源：http://dol.yuanzhike.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ibv.hywenlv.cn

Go:   json.Marshal(obj)
来源：http://cfy.fanxiaobao.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://ibw.daxiang520.top

C#:   JsonSerializer.Serialize(obj)
来源：http://oza.bbcook.cn

[K02] JSON 字符串转对象
来源：http://hit.feifeiyinyue.top

Py:   json.loads(s)
来源：http://dbv.shzxlz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xgk.zdbjq.cn

JS:   JSON.parse(s)
来源：http://evc.zhongyouzk.top

TS:   JSON.parse(s)
来源：http://obq.zhoulong.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ote.shanyushiyangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://euv.yuanzhike.top

Ruby: JSON.parse(s)
来源：http://dto.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://myq.chenzaomai.com

[K03] JSON 美化输出（带缩进）
来源：http://lnf.guannengcc.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bmv.xinyue.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ziy.birdmap.top

JS:   JSON.stringify(obj, null, 2)
来源：http://idr.zhengqikj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://rbg.shanyushiyangkeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dsi.shuidangran.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dkp.yongpay.top

Ruby: JSON.pretty_generate(obj)
来源：http://tcv.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rct.aibaodan.cn

[K04] 读取 JSON 文件
来源：http://oga.ybcxt.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://exn.316326.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tzj.yongpay.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qsr.daria6918.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wmb.feifeiyinyue.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jew.epnwcf.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://glv.chenlongwang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ccl.zhengqikj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qlj.uphjek.com

[K05] 深拷贝对象
来源：http://lzg.nanxinkj.top

Py:   copy.deepcopy(obj)
来源：http://bqb.yueranfly.top

PHP:  unserialize(serialize($obj));
来源：http://pcd.shanyushiyangtech.top

JS:   structuredClone(obj)
来源：http://wfp.aizwys.cn

TS:   structuredClone(obj)
来源：http://auq.zdqjudy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://scy.shuidangran.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ria.tanke756.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ygu.hongshengwenyu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://swe.yvedp.cn

[K06] 解析 URL 查询串
来源：http://mbt.dashuyun.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://muc.gaohongyu789.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vau.yfazqb.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ipd.zdqjudy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eve.hywenlv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mzn.sufxvd.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nfl.shzxlz.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kwn.mhx1999.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lig.feifeiyinyue.top

[K07] 进制转换
来源：http://shu.xziqi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uhw.fengsongda.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tbu.jyoumei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://faw.xingfuxueyuan.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://khv.daria6918.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://egm.yvedp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nrx.aibaodan.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://psf.jinqigufen.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xse.cqqwz.cn

[K08] 二进制序列化（非 JSON）
来源：http://sxk.zhaomingkeji.xyz

Py:   pickle.dumps(obj)
来源：http://zyy.uphjek.com

PHP:  serialize($obj);  unserialize($s);
来源：http://oyn.sufxvd.cn

JS:   v8.serialize(obj)        // Node
来源：http://xof.yanxiufei.cn

TS:   v8.serialize(obj)        // Node
来源：http://bdx.wangdashe.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wqd.c1oappe.top

Go:   encoding/gob
来源：http://anb.hfpthk.cn

Ruby: Marshal.dump(obj)
来源：http://hhn.uphjek.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zxe.cucudq.cn

================================================================================
来源：http://zmv.ydjk.org.cn

L. 网络请求
来源：http://vbw.fktsv.cn

================================================================================
来源：http://yrp.yvedp.cn

[L01] 发送 GET 请求
来源：http://osl.feifeiyinyue.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wjy.wangshuangyany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ugp.ivvv.top

JS:   await fetch(url)
来源：http://qfb.316326.xyz

TS:   await fetch(url)
来源：http://kfr.shangyingyoupin.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gbz.yvedp.cn

Go:   resp, err := http.Get(url)
来源：http://gvc.jinqigfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://rai.xingfuxueyuan.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jvb.havefunace.top

[L02] 发送 POST JSON
来源：http://eni.zhijiandao.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kvn.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rfx.bjfxy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zux.svipenyu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://plx.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vxv.jianghu66.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aty.gaohongyu789.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://onv.chenzaomai.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://caz.yonumen.top

[L03] 设置自定义请求头
来源：http://roa.tanke756.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rjs.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rmf.yongpay.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xoi.zhixingplan.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kvk.zhijiandao.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ksr.316326.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ule.jinghuilouyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xsf.epnwcf.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lda.yangfankeji.com

[L04] 设置超时
来源：http://kid.yanxiufei.cn

Py:   requests.get(url, timeout=5)
来源：http://gwa.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vhc.mhx1999.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zhr.hnxiangtu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oif.9152youxi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bkt.yonumen.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tac.xylfe.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zun.hnxiangtu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cmp.cheryme.top

[L05] 上传文件（multipart）
来源：http://zpz.kuanghao11.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iqm.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yqx.ctjpmb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qxw.sxryk.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gzg.shzxlz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bkn.yj20258888.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dzu.zhijiandao.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qsu.hfpthk.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fdu.yuanzhike.top

[L06] 解析响应为 JSON
来源：http://kcy.dianchejie.cn

Py:   resp.json()
来源：http://eos.epnwcf.com

PHP:  json_decode($body, true);
来源：http://wrr.aizwys.cn

JS:   await resp.json()
来源：http://azm.guannengcc.top

TS:   await resp.json()
来源：http://gkv.ydzc1.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hid.jiagoushi.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://clk.jinqigfzy.top

Ruby: JSON.parse(resp.body)
来源：http://cid.iojbl.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://woa.jyoumei.cn

[L07] 处理 HTTP 状态码
来源：http://qjh.andypj.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yyk.tianlin.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fpw.shuidangran.top

JS:   resp.ok;  resp.status
来源：http://per.fzhhl.top

TS:   resp.ok;  resp.status
来源：http://iqc.jinqigufen.top

Java: resp.statusCode()
来源：http://rbt.vehdjk.com

Go:   resp.StatusCode
来源：http://chi.yj20258888.top

Ruby: resp.code.to_i
来源：http://jaf.ydzc1.top

C#:   (int)resp.StatusCode
来源：http://noy.chenlongwang.top

[L08] 并发请求多个地址
来源：http://cgi.bjfxy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ole.smart0.xyz

PHP:  curl_multi_init() 系列
来源：http://dhr.zdqjudy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://igm.cheryme.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uve.cheryme.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sgt.dashuyun.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eoa.hesvh.cn


<!-- 参考信息 -->