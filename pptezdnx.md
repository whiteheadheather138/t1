代发 wailian999

[I02] 提取所有匹配
来源：http://qqm.yj202588.top

Py:   re.findall(r"\d+", s)
来源：http://feu.iojbl.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hva.ydjk.org.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xmi.jlsjyb.cn

TS:   s.match(/\d+/g)
来源：http://hdc.316326.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pys.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wxm.yuanzhike.top

Ruby: s.scan(/\d+/)
来源：http://slc.tarul.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://eaf.shuidangran.top

[I03] 提取捕获分组
来源：http://lrb.zhijiandao.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dei.ppjwa.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vie.xinyue.icu

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bcq.shangyingyoupin.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dst.yueranfly.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ate.ybcxt.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gyp.zhijiandao.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hyv.bjfxy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rfc.cashguo.top

[I04] 正则替换
来源：http://eio.sufxvd.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dlf.cucudq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pvj.yj20258.top

JS:   s.replace(/\d+/g, "#")
来源：http://ebo.zhijiandao.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ejx.zycfv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xwy.fehbvm.com

Go:   re.ReplaceAllString(s, "#")
来源：http://pga.jlsjyb.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tie.snrcjt.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://top.chenjidiqi.icu

[I05] 按正则拆分
来源：http://kzn.fzhhl.top

Py:   re.split(r"\s*,\s*", s)
来源：http://pkb.epnwcf.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wzd.yongpay.top

JS:   s.split(/\s*,\s*/)
来源：http://zzz.nanxuanxn.top

TS:   s.split(/\s*,\s*/)
来源：http://fgx.nanxinkj.top

Java: s.split("\\s*,\\s*")
来源：http://ttd.ybcxt.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://onl.cheryme.top

Ruby: s.split(/\s*,\s*/)
来源：http://clu.fktsv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tta.tanke756.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zqo.hnqzz.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://adp.vehdjk.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yjs.zhijiandao.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gpk.hammf.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hae.bjfxy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jtv.52xcode.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dyh.316326.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://awz.cqqwz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qeh.sxryk.cn

[I07] 忽略大小写与多行模式
来源：http://fdg.9152youxi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fbz.sysykeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hix.9152youxi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tfe.xziqi.cn

TS:   /error/gim
来源：http://bvn.bbcook.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rcp.nanxinkj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bsm.zdqjudy.top

Ruby: s.scan(/error/i)
来源：http://cvr.cucudq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zfc.zhiwuduotai.top

[I08] 贪婪与非贪婪匹配
来源：http://gpj.ppjwa.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cuj.sweek.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zwx.yonumen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bsw.tanke756.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://etg.ehwqpu.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://cpf.fanxiaobao.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wkl.pengpengdd.cyou

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nsn.yvedp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sxz.gotoacloud.top

================================================================================
来源：http://sod.nanxinkj.top

J. 日期与时间
来源：http://kjy.xziqi.cn

================================================================================
来源：http://wfd.yonumen.top

[J01] 获取当前时间
来源：http://jjt.hnxiangtu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://czj.cheryme.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zol.ivvv.top

JS:   new Date();  Date.now()
来源：http://efb.jianghu66.top

TS:   new Date();  Date.now()
来源：http://kmb.snrcjt.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xph.redwolf501.top

Go:   time.Now()
来源：http://wvx.cdnleiting.top

Ruby: Time.now
来源：http://wnr.jiagoushi.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vbe.aizwys.cn

[J02] 格式化输出
来源：http://kap.yueranfly.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zfs.smart0.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fvs.yj20258.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cxf.chenjidiqi.icu

TS:   d.toISOString()
来源：http://anh.hcnkem.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://crt.tarul.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dpt.pycfn.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wug.shuidangran.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cmy.cucudq.cn

[J03] 字符串解析为日期
来源：http://scr.zdqjudy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qqs.jqgfzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vvu.hysaishi.cn

JS:   new Date("2024-01-02")
来源：http://mlw.sufxvd.cn

TS:   new Date("2024-01-02")
来源：http://ciq.yvedp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xvo.hfpthk.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://aqp.hesvh.cn

Ruby: Date.parse("2024-01-02")
来源：http://mly.zhaomingkeji.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hzh.svipenyu.cn

[J04] 时间戳与日期互转
来源：http://lxp.jqgufenzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bod.wangshuangyany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tqc.vehdjk.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kjx.zdbjq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://uod.zhixingplan.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lyi.sufxvd.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jcp.hongshengwenyu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hgj.fengsongda.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wkq.zdqjudy.top

[J05] 时间加减（加 7 天）
来源：http://rvc.smart0.xyz

Py:   now + timedelta(days=7)
来源：http://iwo.cqqwz.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gvq.jqgfzy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://plo.quarkkingdee.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tzf.nanxinkj.top

Java: LocalDate.now().plusDays(7)
来源：http://nms.fehbvm.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nsp.zycfv.cn

Ruby: Time.now + 7 * 86400
来源：http://xcl.jinyuanbaomall.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nfh.shzxlz.cn

[J06] 计算两时间之差
来源：http://cck.sysykeji.top

Py:   (end - start).total_seconds()
来源：http://xxi.gaohongyu789.top

PHP:  $end->diff($start)->days;
来源：http://chy.yangfankeji.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pdv.smart0.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bic.sxryk.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ynu.quarkkingdee.top

Go:   end.Sub(start).Hours()
来源：http://toz.sweek.top

Ruby: end - start                 # 返回秒数
来源：http://ead.hongshengwenyu.top

C#:   (end - start).TotalSeconds
来源：http://dmw.ywan-chungtsiang.top

[J07] 比较两个日期
来源：http://gvs.snrcjt.cn

Py:   d1 < d2;  d1 == d2
来源：http://pyf.zycfv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gaa.snrcjt.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yfy.52xcode.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gkd.52xcode.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pxd.tian-w.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lwh.gotoacloud.top

Ruby: d1 < d2;  d1 == d2
来源：http://cym.jinghuilouyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://oqp.shangyingyoupin.top

[J08] 提取年月日与星期
来源：http://eiv.gzhubu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://imt.pycfn.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hvv.gogol.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xvp.dashuyun.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://did.sysykeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://atw.jinghuilouyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ljq.jqgufenzy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://omb.chenlongwang.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cjt.bbcook.cn

[J09] 时区处理
来源：http://fhl.hnqzz.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wjn.vqdsnc.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://eop.hcnkem.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://age.uphjek.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xfs.fktsv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qla.yj202588.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://psf.shangyingyoupin.top

Ruby: Time.now.getlocal("+08:00")
来源：http://iaf.kuanghao11.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://npt.yuanzhike.top

[J10] 取今天 / 本月第一天
来源：http://tfb.shanyushiyangtech.top

Py:   date.today();  date.today().replace(day=1)
来源：http://gbw.guowangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kri.sysykeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bbo.ydzc1.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nsy.hcnkem.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hig.xuetiantiany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://acx.guowangkeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bbz.bjfxy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dkv.jqgufenzy.top

================================================================================
来源：http://mxj.ivvv.top

K. JSON 与序列化
来源：http://qoe.zhengqikj.top

================================================================================
来源：http://xeg.zhoulong.xyz

[K01] 对象转 JSON 字符串
来源：http://nds.feifeiyinyue.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sxf.zhiwuduotai.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zcs.guannengcc.top

JS:   JSON.stringify(obj)
来源：http://grb.jinqigfzy.top

TS:   JSON.stringify(obj)
来源：http://geb.guannengcc.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nbp.fengsongda.top

Go:   json.Marshal(obj)
来源：http://gcn.pycfn.com

Ruby: obj.to_json                                     // require "json"
来源：http://thu.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ejn.fehbvm.com

[K02] JSON 字符串转对象
来源：http://sqi.fktsv.cn

Py:   json.loads(s)
来源：http://tdl.shanyushiyangtech.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uwt.zdqjudy.top

JS:   JSON.parse(s)
来源：http://opf.jlsjyb.cn

TS:   JSON.parse(s)
来源：http://rjt.yanxiufei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wfh.fanxiaobao.xyz

Go:   json.Unmarshal(data, &v)
来源：http://tus.yuanzhike.top

Ruby: JSON.parse(s)
来源：http://sfy.bbcook.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xdb.0kj1m.cn

[K03] JSON 美化输出（带缩进）
来源：http://dho.hesvh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://thc.feifeiyinyue.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yki.kuanghao11.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gsw.fktsv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bou.hongshengwenyu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ijl.snrcjt.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zyg.andypj.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://ykh.hesvh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cdu.hcnkem.com

[K04] 读取 JSON 文件
来源：http://ewy.sysykeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gip.ywan-chungtsiang.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fze.jinyuanbaomall.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://inp.zhoulong.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vgt.xuanzx.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zqh.316326.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://scc.zhongyouzk.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://psl.smart0.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ljv.jinqigfzy.top

[K05] 深拷贝对象
来源：http://yww.zhongyouzk.top

Py:   copy.deepcopy(obj)
来源：http://ixd.fzhhl.top

PHP:  unserialize(serialize($obj));
来源：http://rqr.yj20258888.top

JS:   structuredClone(obj)
来源：http://adh.fktsv.cn

TS:   structuredClone(obj)
来源：http://egx.yuanzhike.top

Java: // 手写拷贝构造，或序列化往返
来源：http://pib.c1oappe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xoy.9152youxi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ata.aizwys.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://aiv.zhijiandao.cn

[K06] 解析 URL 查询串
来源：http://cik.shanyushiyangtech.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vkl.yonumen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wkp.fzhhl.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ljt.mhx1999.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wdh.jiagoushi.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hbx.meibo888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://rpw.nanxuanxn.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dze.shzxlz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tjg.c1oappe.top

[K07] 进制转换
来源：http://aeo.zhongyouzk.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cba.hysaishi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tvm.jianghu66.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pkx.zycfv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wrd.jqgfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ayw.kuanghao11.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bry.hfpthk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zvj.0kj1m.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pig.tanke756.top

[K08] 二进制序列化（非 JSON）
来源：http://kva.ybcxt.top

Py:   pickle.dumps(obj)
来源：http://qip.sxryk.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vpl.9152youxi.cn

JS:   v8.serialize(obj)        // Node
来源：http://any.fengsongda.top

TS:   v8.serialize(obj)        // Node
来源：http://wtp.zhixingplan.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dxv.fanxiaobao.xyz

Go:   encoding/gob
来源：http://qko.aibaodan.cn

Ruby: Marshal.dump(obj)
来源：http://kiq.nanxinkj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zaz.yj20258.top

================================================================================
来源：http://lpp.svipenyu.cn

L. 网络请求
来源：http://yjn.zhaomingkeji.xyz

================================================================================
来源：http://zjz.jinqigufen.top

[L01] 发送 GET 请求
来源：http://etg.xingfuxueyuan.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rqu.guannengcc.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://osd.gzhubu.top

JS:   await fetch(url)
来源：http://egz.shangyingyoupin.top

TS:   await fetch(url)
来源：http://zgh.dashuyun.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mos.chenzaomai.com

Go:   resp, err := http.Get(url)
来源：http://tly.ywan-chungtsiang.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ogf.yangfankeji.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oti.mhx1999.top

[L02] 发送 POST JSON
来源：http://kel.sysykeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://kwl.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vok.bbcook.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://niv.dashuyun.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ymc.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xhk.zhoulong.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jhg.xuetiantiany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aus.gogol.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kds.chenzaomai.com

[L03] 设置自定义请求头
来源：http://agy.epnwcf.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yyb.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hyp.quarkkingdee.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lew.ydjk.org.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://swm.jyoumei.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gcr.wangshuangyany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fcr.jinqigfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oeu.zhengqikj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kqh.yanxiufei.cn

[L04] 设置超时
来源：http://hie.zhoulong.xyz

Py:   requests.get(url, timeout=5)
来源：http://djj.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pwh.0kj1m.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hyc.sxryk.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rjg.pengpengdd.cyou

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://weh.jinqigufen.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ehv.xingfuxueyuan.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://txz.sweek.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dbd.haohaochexian.top

[L05] 上传文件（multipart）
来源：http://mhd.jiagoushi.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nrb.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cjm.vehdjk.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xqf.redwolf501.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dhs.jlsjyb.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fsu.zhiwuduotai.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mzo.zdqjudy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://axv.yfazqb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hto.xziqi.cn

[L06] 解析响应为 JSON
来源：http://tnf.guowangkeji.top

Py:   resp.json()
来源：http://kon.shanyushiyangtech.top

PHP:  json_decode($body, true);
来源：http://opg.tarul.cn

JS:   await resp.json()
来源：http://wqf.jqgufenzy.top

TS:   await resp.json()
来源：http://osb.jqgfzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rfu.ywan-chungtsiang.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xrk.zhengqikj.top

Ruby: JSON.parse(resp.body)
来源：http://yms.vehdjk.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xew.fengsongda.top

[L07] 处理 HTTP 状态码
来源：http://eyc.shzxlz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ort.shanyushiyangtech.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://enf.cucudq.cn

JS:   resp.ok;  resp.status
来源：http://vlr.uphjek.com

TS:   resp.ok;  resp.status
来源：http://rih.xylfe.cn

Java: resp.statusCode()
来源：http://fii.zdbjq.cn

Go:   resp.StatusCode
来源：http://lpt.sxryk.cn

Ruby: resp.code.to_i
来源：http://apg.guannengcc.top

C#:   (int)resp.StatusCode
来源：http://nln.zhiwuduotai.top

[L08] 并发请求多个地址
来源：http://cep.ehwqpu.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zly.chenjidiqi.icu

PHP:  curl_multi_init() 系列
来源：http://phn.cashguo.top


<!-- 参考信息 -->