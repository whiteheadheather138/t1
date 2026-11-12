代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://thp.birdmap.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xos.9152youxi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vck.316326.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://llb.jlsjyb.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nun.316326.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vrl.dianchejie.cn

[I04] 正则替换
来源：http://tiv.tanke756.top

Py:   re.sub(r"\d+", "#", s)
来源：http://bpv.kuanghao11.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jwg.bjfxy.top

JS:   s.replace(/\d+/g, "#")
来源：http://zew.iojbl.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nus.chenzaomai.com

Java: s.replaceAll("\\d+", "#")
来源：http://lnf.sweek.top

Go:   re.ReplaceAllString(s, "#")
来源：http://xmd.haohaochexian.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hvc.pycfn.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baz.vqdsnc.cn

[I05] 按正则拆分
来源：http://apw.sjlbkw.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qwd.ywan-chungtsiang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jqq.meibo888.top

JS:   s.split(/\s*,\s*/)
来源：http://qxf.jinqigfzy.top

TS:   s.split(/\s*,\s*/)
来源：http://cuy.wangdashe.top

Java: s.split("\\s*,\\s*")
来源：http://exd.shangyingyoupin.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ymn.shuidangran.top

Ruby: s.split(/\s*,\s*/)
来源：http://qah.zhixingplan.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jfp.chenzaomai.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qcl.svipenyu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qoj.hcnkem.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lpc.gogol.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wxd.tian-w.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mhq.zhaomingkeji.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fsi.chenzaomai.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://neu.jinyuanbaomall.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fxi.nwbrower.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://emn.ppjwa.cn

[I07] 忽略大小写与多行模式
来源：http://ovx.chenjidiqi.icu

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bjb.hesvh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mmi.9152youxi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ksf.cashguo.top

TS:   /error/gim
来源：http://rsv.9152youxi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lig.zhengqikj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lne.jinqigufen.top

Ruby: s.scan(/error/i)
来源：http://fek.feifeiyinyue.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ics.zdbjq.cn

[I08] 贪婪与非贪婪匹配
来源：http://rtr.cheryme.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dnj.zhiwuduotai.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://trh.tianlin.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://znn.nanxinkj.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vyj.yuanzhike.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jik.guannengcc.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rfm.tarul.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rld.zhijiandao.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://unv.jinqigufen.top

================================================================================
来源：http://dej.xuetiantiany.cn

J. 日期与时间
来源：http://iko.zhengqikj.top

================================================================================
来源：http://zdx.yfazqb.com

[J01] 获取当前时间
来源：http://wlp.kuanghao11.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kvf.mhx1999.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nla.wangdashe.top

JS:   new Date();  Date.now()
来源：http://xwu.cqqwz.cn

TS:   new Date();  Date.now()
来源：http://rtm.xinyue.icu

Java: LocalDateTime.now();  Instant.now()
来源：http://ypv.nanxuanxn.top

Go:   time.Now()
来源：http://cfk.zhengqikj.top

Ruby: Time.now
来源：http://xnb.c1oappe.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://giq.hnqzz.top

[J02] 格式化输出
来源：http://iov.epnwcf.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jyb.zhijiandao.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fdn.fktsv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hnh.yonumen.top

TS:   d.toISOString()
来源：http://xdp.hnqzz.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rvt.daxiang520.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://eab.guowangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dsz.jinqigufen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xhr.zhongyouzk.top

[J03] 字符串解析为日期
来源：http://nkf.yj202588.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://szx.cqqwz.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zyz.zycfv.cn

JS:   new Date("2024-01-02")
来源：http://vhd.hammf.cn

TS:   new Date("2024-01-02")
来源：http://pfo.zhaomingkeji.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://kyw.jlsjyb.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uwz.nwbrower.top

Ruby: Date.parse("2024-01-02")
来源：http://gap.nwbrower.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zbf.hesvh.cn

[J04] 时间戳与日期互转
来源：http://qoo.yangfankeji.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://spz.fktsv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fnu.zhijiandao.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ufr.meibo888.top

TS:   Math.floor(Date.now() / 1000)
来源：http://fmf.ppjwa.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://muq.sufxvd.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jvt.yueranfly.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://brz.iojbl.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://utp.mhx1999.top

[J05] 时间加减（加 7 天）
来源：http://njz.quarkkingdee.top

Py:   now + timedelta(days=7)
来源：http://ksf.xuanzx.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://wnl.zhiwuduotai.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qku.sweek.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://suy.shzxlz.cn

Java: LocalDate.now().plusDays(7)
来源：http://fbc.wangshuangyany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dmf.yj202588.top

Ruby: Time.now + 7 * 86400
来源：http://hil.sysykeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://yvd.yj202588.top

[J06] 计算两时间之差
来源：http://hnx.jinghuilouyu.cn

Py:   (end - start).total_seconds()
来源：http://ypx.yfazqb.com

PHP:  $end->diff($start)->days;
来源：http://trv.nanxuanxn.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mvr.ehwqpu.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://haa.havefunace.top

Java: Duration.between(start, end).toSeconds()
来源：http://zcw.52xcode.cn

Go:   end.Sub(start).Hours()
来源：http://wae.sysykeji.top

Ruby: end - start                 # 返回秒数
来源：http://dop.xuanzx.com

C#:   (end - start).TotalSeconds
来源：http://dgm.cheryme.top

[J07] 比较两个日期
来源：http://gum.wangshuangyany.cn

Py:   d1 < d2;  d1 == d2
来源：http://wlx.zhongyouzk.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rad.cucudq.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lqf.wangshuangyany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nvm.shuidangran.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ndq.yj20258888.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://txf.cashguo.top

Ruby: d1 < d2;  d1 == d2
来源：http://hta.guowangkeji.top

C#:   d1 < d2;  d1 == d2
来源：http://ybn.andypj.xyz

[J08] 提取年月日与星期
来源：http://gjt.bjfxy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nad.yongpay.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oyo.sxryk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jth.quarkkingdee.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fnu.ydzc1.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qdl.redwolf501.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gti.c1oappe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rnr.ppjwa.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nxc.cqqwz.cn

[J09] 时区处理
来源：http://zpe.shanyushiyangtech.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ylr.svipenyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cob.yj20258888.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eqe.hcnkem.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nne.meibo888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rhu.sufxvd.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://twa.shanyushiyangtech.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qgn.9152youxi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fkx.hysaishi.cn

[J10] 取今天 / 本月第一天
来源：http://jsd.shuidangran.top

Py:   date.today();  date.today().replace(day=1)
来源：http://kgb.quarkkingdee.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qiy.gotoacloud.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pwu.ybcxt.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fwt.shanyushiyangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lbd.xziqi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://iob.cucudq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://eyz.pengpengdd.cyou

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gmr.dashuyun.cn

================================================================================
来源：http://wss.ywan-chungtsiang.top

K. JSON 与序列化
来源：http://uhk.sysykeji.top

================================================================================
来源：http://wgu.ybcxt.top

[K01] 对象转 JSON 字符串
来源：http://vkk.52xcode.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ukd.tianlin.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gpp.nwbrower.top

JS:   JSON.stringify(obj)
来源：http://urx.nwbrower.top

TS:   JSON.stringify(obj)
来源：http://kus.hammf.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://juh.ctjpmb.com

Go:   json.Marshal(obj)
来源：http://vwv.hnxiangtu.top

Ruby: obj.to_json                                     // require "json"
来源：http://oup.hnqzz.top

C#:   JsonSerializer.Serialize(obj)
来源：http://yon.shuidangran.top

[K02] JSON 字符串转对象
来源：http://boh.gogol.net.cn

Py:   json.loads(s)
来源：http://vqx.feifeiyinyue.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hpo.316326.xyz

JS:   JSON.parse(s)
来源：http://fsb.zdbjq.cn

TS:   JSON.parse(s)
来源：http://mng.zhixingplan.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zsz.quarkkingdee.top

Go:   json.Unmarshal(data, &v)
来源：http://eph.hfpthk.cn

Ruby: JSON.parse(s)
来源：http://wej.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nkc.vehdjk.com

[K03] JSON 美化输出（带缩进）
来源：http://cpd.gogol.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jgc.yonumen.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gtw.tianlin.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://uoe.ydjk.org.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fhq.ydjk.org.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://chh.yfazqb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ybr.yangfankeji.com

Ruby: JSON.pretty_generate(obj)
来源：http://itp.sufxvd.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ida.shanyushiyangkeji.top

[K04] 读取 JSON 文件
来源：http://ilj.uphjek.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hig.svipenyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lho.fehbvm.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lsi.pycfn.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gxc.vqdsnc.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uvb.ppjwa.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dsk.ywan-chungtsiang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://owh.pengpengdd.cyou

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lxd.aizwys.cn

[K05] 深拷贝对象
来源：http://obk.shangyingyoupin.top

Py:   copy.deepcopy(obj)
来源：http://oen.ybcxt.top

PHP:  unserialize(serialize($obj));
来源：http://yii.ivvv.top

JS:   structuredClone(obj)
来源：http://qpt.zdbjq.cn

TS:   structuredClone(obj)
来源：http://jvc.yongpay.top

Java: // 手写拷贝构造，或序列化往返
来源：http://hhy.jqgfzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hyy.gogol.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zew.jinghuilouyu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xog.zdqjudy.top

[K06] 解析 URL 查询串
来源：http://xtb.hongshengwenyu.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tts.jinghuilouyu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ewp.zhijiandao.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pci.vqdsnc.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bix.daxiang520.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hue.zhijiandao.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tpd.jyoumei.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jig.tian-w.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wtg.shangyingyoupin.top

[K07] 进制转换
来源：http://vzk.316326.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jkn.hesvh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hgh.cashguo.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uyy.zhiwuduotai.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nqq.ydzc1.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kbf.ppjwa.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ohv.shangyingyoupin.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vta.yj20258888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://aow.smart0.xyz

[K08] 二进制序列化（非 JSON）
来源：http://wpt.fktsv.cn

Py:   pickle.dumps(obj)
来源：http://etj.bbcook.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hvk.zhoulong.xyz

JS:   v8.serialize(obj)        // Node
来源：http://ffg.shangyingyoupin.top

TS:   v8.serialize(obj)        // Node
来源：http://whf.yfazqb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://roq.jqgufenzy.top

Go:   encoding/gob
来源：http://xya.haohaochexian.top

Ruby: Marshal.dump(obj)
来源：http://psr.shangyingyoupin.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dqp.ppjwa.cn

================================================================================
来源：http://euj.zhaomingkeji.xyz

L. 网络请求
来源：http://jpj.hcnkem.com

================================================================================
来源：http://nzr.wangshuangyany.cn

[L01] 发送 GET 请求
来源：http://wbl.bbcook.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lto.pengpengdd.cyou

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lxn.cdnleiting.top

JS:   await fetch(url)
来源：http://sxa.shzxlz.cn

TS:   await fetch(url)
来源：http://scx.chenlongwang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lbb.zdbjq.cn

Go:   resp, err := http.Get(url)
来源：http://ucc.jinghuilouyu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zdi.shanyushiyangkeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://csb.hesvh.cn

[L02] 发送 POST JSON
来源：http://yjp.52xcode.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fnp.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mjg.dashuyun.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://spe.pengpengdd.cyou

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qkg.yanxiufei.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sle.wangdashe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qvt.pengpengdd.cyou

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rna.ydzc1.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mxb.guowangkeji.top

[L03] 设置自定义请求头
来源：http://liu.ybcxt.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mti.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zaw.chenzaomai.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qpg.zhiwuduotai.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://flk.wangshuangyany.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cfh.fehbvm.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rgs.hfpthk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iat.dianchejie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yfy.cashguo.top

[L04] 设置超时
来源：http://rub.pengpengdd.cyou

Py:   requests.get(url, timeout=5)
来源：http://lbd.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://joj.52xcode.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ajn.shanyushiyangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://swf.iojbl.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ftj.zhijiandao.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tbt.yfazqb.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fcn.guowangkeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zcq.ywan-chungtsiang.top

[L05] 上传文件（multipart）
来源：http://cmk.shanyushiyangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uxk.sweek.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pxj.jqgufenzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kvl.snrcjt.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xoa.chenzaomai.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pci.zhixingplan.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uxy.nanxinkj.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nkt.zdbjq.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tiu.iojbl.cn

[L06] 解析响应为 JSON
来源：http://xlr.shzxlz.cn

Py:   resp.json()
来源：http://fmz.yongpay.top

PHP:  json_decode($body, true);
来源：http://tun.gotoacloud.top

JS:   await resp.json()
来源：http://kos.yuxming.cn

TS:   await resp.json()
来源：http://ifz.yueranfly.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rpg.tian-w.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ywz.yj202588.top

Ruby: JSON.parse(resp.body)
来源：http://gqg.guowangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mzt.nanxuanxn.top

[L07] 处理 HTTP 状态码
来源：http://nci.9152youxi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://geg.pengpengdd.cyou

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wst.daxiang520.top

JS:   resp.ok;  resp.status
来源：http://lup.xingfuxueyuan.xyz

TS:   resp.ok;  resp.status
来源：http://keb.yj20258.top

Java: resp.statusCode()
来源：http://bzb.shanyushiyangtech.top

Go:   resp.StatusCode
来源：http://epd.gaohongyu789.top

Ruby: resp.code.to_i
来源：http://rsw.meibo888.top

C#:   (int)resp.StatusCode
来源：http://daf.c1oappe.top

[L08] 并发请求多个地址
来源：http://rfh.chenlongwang.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://htc.yuxming.cn

PHP:  curl_multi_init() 系列
来源：http://wmt.jyoumei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nvu.gaohongyu789.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jpu.xingfuxueyuan.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fif.tianlin.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hcp.bbcook.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vzn.fengsongda.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qdn.dashuyun.cn

================================================================================
来源：http://ncr.0kj1m.cn

M. 命令行 / 进程 / 环境
来源：http://dcm.jianghu66.top

================================================================================
来源：http://gzd.xuanzx.com

[M01] 读取命令行参数
来源：http://sab.haohaochexian.top

Py:   sys.argv[1:]
来源：http://gdw.zhengqikj.top

PHP:  $argv;  $argc;
来源：http://eiq.nwbrower.top


<!-- 参考信息 -->