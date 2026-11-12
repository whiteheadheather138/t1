代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://act.chenlongwang.top

[I03] 提取捕获分组
来源：http://etn.jqgfzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://evd.jinqigufen.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://meb.ehwqpu.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://svx.zhijiandao.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pzg.gotoacloud.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pin.zhiwuduotai.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lmy.tianlin.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rdz.zdqjudy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yda.ctjpmb.com

[I04] 正则替换
来源：http://hxm.ybcxt.top

Py:   re.sub(r"\d+", "#", s)
来源：http://bnt.wangdashe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ogw.xingfuxueyuan.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://ygg.jlsjyb.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hvp.jinghuilouyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jiz.zhijiandao.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lcm.shuidangran.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ccb.shuidangran.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://owy.gogol.net.cn

[I05] 按正则拆分
来源：http://oqn.zhijiandao.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tbi.52xcode.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://avd.chenzaomai.com

JS:   s.split(/\s*,\s*/)
来源：http://qnp.sweek.top

TS:   s.split(/\s*,\s*/)
来源：http://kxv.jqgufenzy.top

Java: s.split("\\s*,\\s*")
来源：http://wui.havefunace.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xem.nanxuanxn.top

Ruby: s.split(/\s*,\s*/)
来源：http://xhp.epnwcf.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xvx.zdbjq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yds.yongpay.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cmu.sxryk.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kof.wangdashe.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dht.xuetiantiany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://htu.yuxming.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ahd.c1oappe.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://quw.hongshengwenyu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://stv.svipenyu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://owm.zhongyouzk.top

[I07] 忽略大小写与多行模式
来源：http://qxy.zycfv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gwb.yfazqb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zwv.sufxvd.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xzc.vehdjk.com

TS:   /error/gim
来源：http://hzs.pycfn.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qim.jyoumei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vur.wangshuangyany.cn

Ruby: s.scan(/error/i)
来源：http://hgo.nwbrower.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://slf.wangshuangyany.cn

[I08] 贪婪与非贪婪匹配
来源：http://qvn.hongshengwenyu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xww.aizwys.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://teq.jqgfzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wax.aizwys.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lut.jinqigfzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://zzy.chenzaomai.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zjk.jyoumei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://faa.zdbjq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vqd.zhixingplan.top

================================================================================
来源：http://dth.cashguo.top

J. 日期与时间
来源：http://fry.hfpthk.cn

================================================================================
来源：http://sya.ywan-chungtsiang.top

[J01] 获取当前时间
来源：http://iky.hesvh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pue.zhoulong.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lco.zdbjq.cn

JS:   new Date();  Date.now()
来源：http://qgz.shangyingyoupin.top

TS:   new Date();  Date.now()
来源：http://kyw.hongshengwenyu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dtn.smart0.xyz

Go:   time.Now()
来源：http://aor.sufxvd.cn

Ruby: Time.now
来源：http://hmt.ybcxt.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wpx.zhijiandao.cn

[J02] 格式化输出
来源：http://vyr.yj20258.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qsj.zhengqikj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://btl.yvedp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wlx.dianchejie.cn

TS:   d.toISOString()
来源：http://miq.yanxiufei.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fjh.haohaochexian.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lks.epnwcf.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kcs.uphjek.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ypa.c1oappe.top

[J03] 字符串解析为日期
来源：http://uqs.hnqzz.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xyk.yangfankeji.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gqq.vqdsnc.cn

JS:   new Date("2024-01-02")
来源：http://xli.jinqigfzy.top

TS:   new Date("2024-01-02")
来源：http://rah.zhongyouzk.top

Java: LocalDate.parse("2024-01-02")
来源：http://dfv.mhx1999.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pmz.hysaishi.cn

Ruby: Date.parse("2024-01-02")
来源：http://clc.yvedp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pul.aizwys.cn

[J04] 时间戳与日期互转
来源：http://bnz.birdmap.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ohq.chenjidiqi.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vyh.hnqzz.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ojf.gogol.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://all.vqdsnc.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mpl.zdqjudy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://suf.yangfankeji.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://owh.hfpthk.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://amz.zhaomingkeji.xyz

[J05] 时间加减（加 7 天）
来源：http://izh.hysaishi.cn

Py:   now + timedelta(days=7)
来源：http://gip.aizwys.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sbo.hesvh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://goi.ywan-chungtsiang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://inw.jianghu66.top

Java: LocalDate.now().plusDays(7)
来源：http://gcq.sweek.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sdi.xinyue.icu

Ruby: Time.now + 7 * 86400
来源：http://llq.cdnleiting.top

C#:   DateTime.Now.AddDays(7)
来源：http://kwk.zhongyouzk.top

[J06] 计算两时间之差
来源：http://emw.9152youxi.cn

Py:   (end - start).total_seconds()
来源：http://vqe.tianlin.xyz

PHP:  $end->diff($start)->days;
来源：http://zij.sxryk.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rlf.hnxiangtu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qbu.zhiwuduotai.top

Java: Duration.between(start, end).toSeconds()
来源：http://amr.chenzaomai.com

Go:   end.Sub(start).Hours()
来源：http://ntp.tanke756.top

Ruby: end - start                 # 返回秒数
来源：http://kup.yj20258.top

C#:   (end - start).TotalSeconds
来源：http://jqb.vehdjk.com

[J07] 比较两个日期
来源：http://okr.sxryk.cn

Py:   d1 < d2;  d1 == d2
来源：http://nsq.sxryk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zjs.zycfv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hpz.gogol.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lmf.cashguo.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ymu.daria6918.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nba.shanyushiyangtech.top

Ruby: d1 < d2;  d1 == d2
来源：http://fbp.sweek.top

C#:   d1 < d2;  d1 == d2
来源：http://yyy.quarkkingdee.top

[J08] 提取年月日与星期
来源：http://ian.jiagoushi.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://okq.zhixingplan.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nho.ybcxt.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kqa.hnqzz.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mic.cheryme.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gkb.jianghu66.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qrb.daxiang520.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ivw.ehwqpu.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uum.pycfn.com

[J09] 时区处理
来源：http://pir.bjfxy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xso.dashuyun.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://exc.cheryme.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pxt.dianchejie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://scg.sjlbkw.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vxm.epnwcf.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cpq.yj202588.top

Ruby: Time.now.getlocal("+08:00")
来源：http://agx.quarkkingdee.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mza.zhoulong.xyz

[J10] 取今天 / 本月第一天
来源：http://rvl.jiagoushi.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rzc.jinyuanbaomall.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tyw.jiagoushi.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qte.cashguo.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ymq.nwbrower.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://inb.ivvv.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ula.hongshengwenyu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hmp.gzhubu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nni.yj20258888.top

================================================================================
来源：http://ovi.shangyingyoupin.top

K. JSON 与序列化
来源：http://gin.ctjpmb.com

================================================================================
来源：http://gfp.fktsv.cn

[K01] 对象转 JSON 字符串
来源：http://iht.zhengqikj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wcv.shangyingyoupin.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://urj.yonumen.top

JS:   JSON.stringify(obj)
来源：http://gjs.gaohongyu789.top

TS:   JSON.stringify(obj)
来源：http://vgh.yonumen.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://opn.ywan-chungtsiang.top

Go:   json.Marshal(obj)
来源：http://lic.316326.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://mhb.daria6918.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ybe.yvedp.cn

[K02] JSON 字符串转对象
来源：http://kav.gzhubu.top

Py:   json.loads(s)
来源：http://wzh.jianghu66.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rde.kuanghao11.cn

JS:   JSON.parse(s)
来源：http://tfr.hnxiangtu.top

TS:   JSON.parse(s)
来源：http://vnj.hcnkem.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qkj.0kj1m.cn

Go:   json.Unmarshal(data, &v)
来源：http://sdq.cqqwz.cn

Ruby: JSON.parse(s)
来源：http://fpq.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wlf.guannengcc.top

[K03] JSON 美化输出（带缩进）
来源：http://kzv.guowangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://iql.316326.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iqw.zycfv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zuo.snrcjt.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gpo.sysykeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hir.vqdsnc.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dvv.mhx1999.top

Ruby: JSON.pretty_generate(obj)
来源：http://awi.yuanzhike.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ycl.hnxiangtu.top

[K04] 读取 JSON 文件
来源：http://ugm.vqdsnc.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qcj.fanxiaobao.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jnw.ybcxt.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ylt.jinqigufen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ooj.nanxuanxn.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://izl.birdmap.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nwe.fzhhl.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://uil.fehbvm.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mza.xziqi.cn

[K05] 深拷贝对象
来源：http://pyw.guowangkeji.top

Py:   copy.deepcopy(obj)
来源：http://lgj.gaohongyu789.top

PHP:  unserialize(serialize($obj));
来源：http://tih.shzxlz.cn

JS:   structuredClone(obj)
来源：http://cyg.cashguo.top

TS:   structuredClone(obj)
来源：http://nhe.sjlbkw.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://glb.pycfn.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://soa.chenlongwang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oto.xuanzx.com

C#:   // 序列化往返，或自定义 Clone
来源：http://ecn.nanxuanxn.top

[K06] 解析 URL 查询串
来源：http://hms.zhoulong.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qhx.sweek.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tsa.zdqjudy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dpv.sxryk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hhw.tarul.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cso.cashguo.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://obb.xylfe.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wix.jlsjyb.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tkv.yuxming.cn

[K07] 进制转换
来源：http://hcl.sweek.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://adl.hfpthk.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rvk.gogol.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://eha.xuanzx.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wtv.xylfe.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://aut.yueranfly.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://evj.zdbjq.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pzc.cashguo.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qom.dashuyun.cn

[K08] 二进制序列化（非 JSON）
来源：http://imv.gogol.net.cn

Py:   pickle.dumps(obj)
来源：http://zqo.c1oappe.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ixs.yongpay.top

JS:   v8.serialize(obj)        // Node
来源：http://ufr.fzhhl.top

TS:   v8.serialize(obj)        // Node
来源：http://fbb.xuanzx.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jkf.shanyushiyangkeji.top

Go:   encoding/gob
来源：http://vlj.bjfxy.top

Ruby: Marshal.dump(obj)
来源：http://nzu.shuidangran.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zqr.yangfankeji.com

================================================================================
来源：http://tjo.nanxuanxn.top

L. 网络请求
来源：http://wpo.jiagoushi.top

================================================================================
来源：http://boy.quarkkingdee.top

[L01] 发送 GET 请求
来源：http://oex.gzhubu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wrd.hammf.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ezu.jyoumei.cn

JS:   await fetch(url)
来源：http://xjx.hongshengwenyu.top

TS:   await fetch(url)
来源：http://dkm.nanxinkj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jgv.fzhhl.top

Go:   resp, err := http.Get(url)
来源：http://nsq.yj20258888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://mxk.iojbl.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gyk.jianghu66.top

[L02] 发送 POST JSON
来源：http://hwu.meibo888.top

Py:   requests.post(url, json={"a": 1})
来源：http://cvk.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cge.birdmap.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ioz.fehbvm.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wma.jyoumei.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yaw.zhengqikj.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jik.pycfn.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cbj.meibo888.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pdi.ctjpmb.com

[L03] 设置自定义请求头
来源：http://jmp.ehwqpu.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gmi.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jst.c1oappe.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vfu.sysykeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eyn.vehdjk.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fpj.hfpthk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://llc.hfpthk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uyp.xinyue.icu

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ypb.hammf.cn

[L04] 设置超时
来源：http://qdp.snrcjt.cn

Py:   requests.get(url, timeout=5)
来源：http://iyv.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ypt.iojbl.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nyu.hesvh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://myj.pycfn.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xlk.wangshuangyany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pzz.jqgfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://iat.daxiang520.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ptf.daxiang520.top

[L05] 上传文件（multipart）
来源：http://qaw.fanxiaobao.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nrh.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ger.shanyushiyangkeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://duz.ydjk.org.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://txb.guannengcc.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://aon.havefunace.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mdb.ydjk.org.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gsm.xuetiantiany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wce.pengpengdd.cyou

[L06] 解析响应为 JSON
来源：http://wla.yj20258.top

Py:   resp.json()
来源：http://wss.xuetiantiany.cn

PHP:  json_decode($body, true);
来源：http://nli.chenjidiqi.icu

JS:   await resp.json()
来源：http://kpv.yj20258.top

TS:   await resp.json()
来源：http://qxk.pengpengdd.cyou

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sok.epnwcf.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gct.ywan-chungtsiang.top

Ruby: JSON.parse(resp.body)
来源：http://eoo.ybcxt.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://juz.nanxuanxn.top

[L07] 处理 HTTP 状态码
来源：http://zac.hywenlv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://had.shzxlz.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lei.c1oappe.top

JS:   resp.ok;  resp.status
来源：http://txk.xuetiantiany.cn

TS:   resp.ok;  resp.status
来源：http://eqs.sufxvd.cn

Java: resp.statusCode()
来源：http://kfp.52xcode.cn

Go:   resp.StatusCode
来源：http://hzy.hnqzz.top

Ruby: resp.code.to_i
来源：http://avo.chenzaomai.com

C#:   (int)resp.StatusCode
来源：http://zrn.hywenlv.cn

[L08] 并发请求多个地址
来源：http://czu.pengpengdd.cyou

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://erf.ybcxt.top

PHP:  curl_multi_init() 系列
来源：http://kll.shanyushiyangtech.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cgi.uphjek.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tih.cashguo.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qnm.zhongyouzk.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pxv.hnqzz.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://epw.jinghuilouyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hjd.yangfankeji.com

================================================================================
来源：http://oaj.nwbrower.top

M. 命令行 / 进程 / 环境
来源：http://qoq.zhiwuduotai.top


<!-- 参考信息 -->