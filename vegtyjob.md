代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ppf.zhiwuduotai.top

[I03] 提取捕获分组
来源：http://inw.smart0.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wme.kuanghao11.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yup.cqqwz.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dux.yfazqb.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://all.hcnkem.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://eag.shanyushiyangtech.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://coy.nwbrower.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hma.yfazqb.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ski.zdbjq.cn

[I04] 正则替换
来源：http://zir.yangfankeji.com

Py:   re.sub(r"\d+", "#", s)
来源：http://oih.shangyingyoupin.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://aib.ywan-chungtsiang.top

JS:   s.replace(/\d+/g, "#")
来源：http://fpi.hywenlv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pec.pengpengdd.cyou

Java: s.replaceAll("\\d+", "#")
来源：http://ecr.xziqi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://djb.yj202588.top

Ruby: s.gsub(/\d+/, "#")
来源：http://toi.vqdsnc.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ljk.yongpay.top

[I05] 按正则拆分
来源：http://vtq.xuanzx.com

Py:   re.split(r"\s*,\s*", s)
来源：http://pay.shangyingyoupin.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dtk.0kj1m.cn

JS:   s.split(/\s*,\s*/)
来源：http://ubd.smart0.xyz

TS:   s.split(/\s*,\s*/)
来源：http://hkz.aizwys.cn

Java: s.split("\\s*,\\s*")
来源：http://glx.bbcook.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sil.yj202588.top

Ruby: s.split(/\s*,\s*/)
来源：http://usi.redwolf501.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ida.yuanzhike.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bte.gogol.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fsl.xziqi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jva.zycfv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kck.shanyushiyangtech.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nkf.jqgfzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pjk.feifeiyinyue.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vwm.tarul.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rqx.redwolf501.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://olz.haohaochexian.top

[I07] 忽略大小写与多行模式
来源：http://sdf.jqgufenzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bvg.shanyushiyangtech.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://onl.zhoulong.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://esf.wangdashe.top

TS:   /error/gim
来源：http://mey.hesvh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xgv.iojbl.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://idm.aibaodan.cn

Ruby: s.scan(/error/i)
来源：http://ilk.sufxvd.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ggg.hfpthk.cn

[I08] 贪婪与非贪婪匹配
来源：http://anr.redwolf501.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rpd.cheryme.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qlv.hysaishi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pdr.hywenlv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jvv.ehwqpu.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://fax.0kj1m.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ifs.yueranfly.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sxo.pengpengdd.cyou

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lhe.sufxvd.cn

================================================================================
来源：http://ymc.yfazqb.com

J. 日期与时间
来源：http://cdg.yongpay.top

================================================================================
来源：http://wum.hnqzz.top

[J01] 获取当前时间
来源：http://out.zhijiandao.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fhc.yj20258888.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zid.tian-w.cn

JS:   new Date();  Date.now()
来源：http://bcl.ehwqpu.com

TS:   new Date();  Date.now()
来源：http://pqr.wangdashe.top

Java: LocalDateTime.now();  Instant.now()
来源：http://flg.zhoulong.xyz

Go:   time.Now()
来源：http://ixe.zhongyouzk.top

Ruby: Time.now
来源：http://gxk.hammf.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zgp.gotoacloud.top

[J02] 格式化输出
来源：http://skg.daria6918.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mir.fanxiaobao.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jrj.xylfe.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xjm.hywenlv.cn

TS:   d.toISOString()
来源：http://ptd.zhongyouzk.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tid.iojbl.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://beg.uphjek.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://czr.cqqwz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://udb.zhaomingkeji.xyz

[J03] 字符串解析为日期
来源：http://gnn.yvedp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kbn.yuanzhike.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dku.snrcjt.cn

JS:   new Date("2024-01-02")
来源：http://qgo.birdmap.top

TS:   new Date("2024-01-02")
来源：http://gif.xinyue.icu

Java: LocalDate.parse("2024-01-02")
来源：http://nlm.uphjek.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ypg.snrcjt.cn

Ruby: Date.parse("2024-01-02")
来源：http://qoh.havefunace.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ovh.hesvh.cn

[J04] 时间戳与日期互转
来源：http://iuo.wangshuangyany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mrs.svipenyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lnt.chenlongwang.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ycb.uphjek.com

TS:   Math.floor(Date.now() / 1000)
来源：http://aah.cheryme.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ubw.cqqwz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vzf.yuanzhike.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ysk.yvedp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rxc.yanxiufei.cn

[J05] 时间加减（加 7 天）
来源：http://dwc.hfpthk.cn

Py:   now + timedelta(days=7)
来源：http://plo.shanyushiyangtech.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jtb.9152youxi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pkm.yuanzhike.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://shr.cheryme.top

Java: LocalDate.now().plusDays(7)
来源：http://wjb.redwolf501.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bnz.52xcode.cn

Ruby: Time.now + 7 * 86400
来源：http://hql.yfazqb.com

C#:   DateTime.Now.AddDays(7)
来源：http://bkt.yonumen.top

[J06] 计算两时间之差
来源：http://vsp.hfpthk.cn

Py:   (end - start).total_seconds()
来源：http://nck.sysykeji.top

PHP:  $end->diff($start)->days;
来源：http://kys.wangshuangyany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vmk.quarkkingdee.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tuo.jianghu66.top

Java: Duration.between(start, end).toSeconds()
来源：http://whk.zhixingplan.top

Go:   end.Sub(start).Hours()
来源：http://xvt.daria6918.cn

Ruby: end - start                 # 返回秒数
来源：http://fve.ehwqpu.com

C#:   (end - start).TotalSeconds
来源：http://pbd.shzxlz.cn

[J07] 比较两个日期
来源：http://nfo.sweek.top

Py:   d1 < d2;  d1 == d2
来源：http://rbo.tianlin.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ecy.aibaodan.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hep.zhijiandao.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xrq.hammf.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wjl.xylfe.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hym.zhijiandao.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xkl.havefunace.top

C#:   d1 < d2;  d1 == d2
来源：http://lpj.gogol.net.cn

[J08] 提取年月日与星期
来源：http://pak.fanxiaobao.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cyg.andypj.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ifu.ybcxt.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zxm.yuanzhike.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uyo.yj202588.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lmi.jiagoushi.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vqs.sysykeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://joz.smart0.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jwp.zycfv.cn

[J09] 时区处理
来源：http://aht.yfazqb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fye.yj20258.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lcn.dashuyun.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://npp.fengsongda.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dkl.gotoacloud.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mld.aizwys.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ued.hysaishi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://igq.chenzaomai.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yfy.ivvv.top

[J10] 取今天 / 本月第一天
来源：http://mog.aizwys.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lnk.xylfe.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pxq.jiagoushi.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rwq.chenzaomai.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ldm.nanxuanxn.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lma.jiagoushi.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tqb.nanxuanxn.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fii.shangyingyoupin.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qvf.hammf.cn

================================================================================
来源：http://jzr.c1oappe.top

K. JSON 与序列化
来源：http://vmx.yfazqb.com

================================================================================
来源：http://uds.nanxinkj.top

[K01] 对象转 JSON 字符串
来源：http://cwe.ivvv.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qiz.chenjidiqi.icu

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qvp.nwbrower.top

JS:   JSON.stringify(obj)
来源：http://fms.ybcxt.top

TS:   JSON.stringify(obj)
来源：http://eyh.hysaishi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://icv.dashuyun.cn

Go:   json.Marshal(obj)
来源：http://sdy.xuanzx.com

Ruby: obj.to_json                                     // require "json"
来源：http://qkp.sufxvd.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qgb.jianghu66.top

[K02] JSON 字符串转对象
来源：http://hup.jianghu66.top

Py:   json.loads(s)
来源：http://pkm.yj20258888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fay.guannengcc.top

JS:   JSON.parse(s)
来源：http://hff.snrcjt.cn

TS:   JSON.parse(s)
来源：http://bwk.smart0.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uyd.tarul.cn

Go:   json.Unmarshal(data, &v)
来源：http://uxn.fengsongda.top

Ruby: JSON.parse(s)
来源：http://rka.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xbj.pycfn.com

[K03] JSON 美化输出（带缩进）
来源：http://mga.sufxvd.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://foq.xziqi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lis.ydjk.org.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ycj.smart0.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://ilj.havefunace.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qln.bjfxy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bdh.xziqi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vhq.sufxvd.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://waw.fktsv.cn

[K04] 读取 JSON 文件
来源：http://nfp.hfpthk.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wxd.sxryk.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gyw.yfazqb.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zsr.mhx1999.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pee.fktsv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nci.mhx1999.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://axu.yonumen.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://orw.yj20258.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jdb.shuidangran.top

[K05] 深拷贝对象
来源：http://lhw.yuxming.cn

Py:   copy.deepcopy(obj)
来源：http://lxj.shangyingyoupin.top

PHP:  unserialize(serialize($obj));
来源：http://mtc.sysykeji.top

JS:   structuredClone(obj)
来源：http://uzc.zycfv.cn

TS:   structuredClone(obj)
来源：http://ush.xuanzx.com

Java: // 手写拷贝构造，或序列化往返
来源：http://lro.zycfv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uhv.mhx1999.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wpb.meibo888.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ybv.zdqjudy.top

[K06] 解析 URL 查询串
来源：http://tql.zhiwuduotai.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://guh.yuanzhike.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://omx.zdqjudy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mdq.316326.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://his.smart0.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wva.yuanzhike.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kfw.shuidangran.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zrm.yvedp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zrs.nanxinkj.top

[K07] 进制转换
来源：http://ucm.9152youxi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ovf.birdmap.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cle.hywenlv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gmd.fanxiaobao.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pij.yangfankeji.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lrg.zdbjq.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jpo.yuxming.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wwu.shangyingyoupin.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iww.zhiwuduotai.top

[K08] 二进制序列化（非 JSON）
来源：http://paq.hywenlv.cn

Py:   pickle.dumps(obj)
来源：http://ufd.hongshengwenyu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xzq.jinyuanbaomall.cn

JS:   v8.serialize(obj)        // Node
来源：http://bcn.yj20258888.top

TS:   v8.serialize(obj)        // Node
来源：http://ytk.chenzaomai.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zes.bjfxy.top

Go:   encoding/gob
来源：http://zuk.fehbvm.com

Ruby: Marshal.dump(obj)
来源：http://rey.0kj1m.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dkn.hfpthk.cn

================================================================================
来源：http://nac.xingfuxueyuan.xyz

L. 网络请求
来源：http://sop.cucudq.cn

================================================================================
来源：http://ano.c1oappe.top

[L01] 发送 GET 请求
来源：http://bfy.gaohongyu789.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cro.sufxvd.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ych.fehbvm.com

JS:   await fetch(url)
来源：http://mtb.sweek.top

TS:   await fetch(url)
来源：http://iou.fktsv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qfu.cashguo.top

Go:   resp, err := http.Get(url)
来源：http://cso.ehwqpu.com

Ruby: Net::HTTP.get(URI(url))
来源：http://gre.birdmap.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://feq.kuanghao11.cn

[L02] 发送 POST JSON
来源：http://wxz.shanyushiyangkeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://uau.sweek.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ajl.zhiwuduotai.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nyp.havefunace.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cvp.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kuv.fzhhl.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dqi.mhx1999.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lxr.316326.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nze.yvedp.cn

[L03] 设置自定义请求头
来源：http://clo.ehwqpu.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tfy.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://imo.ppjwa.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zye.feifeiyinyue.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pmr.iojbl.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dpw.ybcxt.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mid.hnqzz.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nxc.meibo888.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://agh.zhijiandao.cn

[L04] 设置超时
来源：http://vbb.pycfn.com

Py:   requests.get(url, timeout=5)
来源：http://xld.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://znm.nanxuanxn.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cvl.zhaomingkeji.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hiy.jiagoushi.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://crn.vehdjk.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xmk.gogol.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nga.yj202588.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vli.chenlongwang.top

[L05] 上传文件（multipart）
来源：http://ggr.yongpay.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eto.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gev.gzhubu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nbh.jinyuanbaomall.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pwr.zhengqikj.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gzx.gzhubu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xna.xingfuxueyuan.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xsv.gaohongyu789.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uqm.ywan-chungtsiang.top

[L06] 解析响应为 JSON
来源：http://sxh.sweek.top

Py:   resp.json()
来源：http://wby.xinyue.icu

PHP:  json_decode($body, true);
来源：http://ndz.epnwcf.com

JS:   await resp.json()
来源：http://nwe.wangdashe.top

TS:   await resp.json()
来源：http://tld.jinqigfzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vdj.bbcook.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hdk.chenzaomai.com

Ruby: JSON.parse(resp.body)
来源：http://jmg.52xcode.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ykz.ehwqpu.com

[L07] 处理 HTTP 状态码
来源：http://rjg.ydzc1.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://azl.dianchejie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gbv.yonumen.top

JS:   resp.ok;  resp.status
来源：http://zem.wangdashe.top

TS:   resp.ok;  resp.status
来源：http://ifj.tarul.cn

Java: resp.statusCode()
来源：http://rgi.gotoacloud.top

Go:   resp.StatusCode
来源：http://cbz.tarul.cn

Ruby: resp.code.to_i
来源：http://owr.chenjidiqi.icu

C#:   (int)resp.StatusCode
来源：http://hjn.shanyushiyangkeji.top

[L08] 并发请求多个地址
来源：http://dvh.hfpthk.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bou.uphjek.com

PHP:  curl_multi_init() 系列
来源：http://tii.hongshengwenyu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xkp.jinyuanbaomall.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nwj.feifeiyinyue.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jpy.yuanzhike.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nvv.jqgufenzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bis.ywan-chungtsiang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cpa.smart0.xyz

================================================================================
来源：http://rld.zhengqikj.top

M. 命令行 / 进程 / 环境
来源：http://fhr.chenzaomai.com


<!-- 参考信息 -->