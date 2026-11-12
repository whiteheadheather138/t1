代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://exo.gaohongyu789.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hho.uphjek.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wzx.xinyue.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mho.aibaodan.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yzf.kuanghao11.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qfa.cucudq.cn

[I04] 正则替换
来源：http://num.sysykeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ywy.snrcjt.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zuv.quarkkingdee.top

JS:   s.replace(/\d+/g, "#")
来源：http://hrs.yueranfly.top

TS:   s.replace(/\d+/g, "#")
来源：http://qhc.yonumen.top

Java: s.replaceAll("\\d+", "#")
来源：http://dtd.birdmap.top

Go:   re.ReplaceAllString(s, "#")
来源：http://lnl.dianchejie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://brc.guannengcc.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ahk.jqgfzy.top

[I05] 按正则拆分
来源：http://uky.9152youxi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://abc.ctjpmb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://huk.yj20258888.top

JS:   s.split(/\s*,\s*/)
来源：http://dqa.nwbrower.top

TS:   s.split(/\s*,\s*/)
来源：http://xqg.cucudq.cn

Java: s.split("\\s*,\\s*")
来源：http://wrn.xuetiantiany.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ots.ppjwa.cn

Ruby: s.split(/\s*,\s*/)
来源：http://kak.sjlbkw.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://skw.ehwqpu.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ihp.yueranfly.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ksi.hammf.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vio.gogol.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fox.wangdashe.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ojv.ydjk.org.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qgo.xziqi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ozj.aizwys.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://khi.ivvv.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hkf.nanxuanxn.top

[I07] 忽略大小写与多行模式
来源：http://twi.cucudq.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lbw.vehdjk.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qpp.svipenyu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lub.smart0.xyz

TS:   /error/gim
来源：http://vci.yvedp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qgv.shuidangran.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ujm.shangyingyoupin.top

Ruby: s.scan(/error/i)
来源：http://fse.dianchejie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jgl.daria6918.cn

[I08] 贪婪与非贪婪匹配
来源：http://pwt.jiagoushi.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uvi.mhx1999.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pxv.hongshengwenyu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sfy.vqdsnc.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://phy.birdmap.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://sou.sweek.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vfi.sjlbkw.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eds.yvedp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cin.fengsongda.top

================================================================================
来源：http://zfp.jianghu66.top

J. 日期与时间
来源：http://mzt.hfpthk.cn

================================================================================
来源：http://jbf.jinghuilouyu.cn

[J01] 获取当前时间
来源：http://rxr.zhoulong.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://ixz.haohaochexian.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lxx.pycfn.com

JS:   new Date();  Date.now()
来源：http://sbl.chenlongwang.top

TS:   new Date();  Date.now()
来源：http://zvz.cashguo.top

Java: LocalDateTime.now();  Instant.now()
来源：http://uae.52xcode.cn

Go:   time.Now()
来源：http://vht.nanxinkj.top

Ruby: Time.now
来源：http://rjd.xingfuxueyuan.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rqj.vqdsnc.cn

[J02] 格式化输出
来源：http://gaw.nwbrower.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ekj.cucudq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://noo.kuanghao11.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aug.fzhhl.top

TS:   d.toISOString()
来源：http://yid.fktsv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gmq.xinyue.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cmm.yuanzhike.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qhs.svipenyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://smd.fehbvm.com

[J03] 字符串解析为日期
来源：http://vih.shuidangran.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dmq.kuanghao11.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sqv.wangshuangyany.cn

JS:   new Date("2024-01-02")
来源：http://xvw.hysaishi.cn

TS:   new Date("2024-01-02")
来源：http://qwk.hnxiangtu.top

Java: LocalDate.parse("2024-01-02")
来源：http://yyh.jinqigfzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bdx.hesvh.cn

Ruby: Date.parse("2024-01-02")
来源：http://vbj.ppjwa.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tuz.chenlongwang.top

[J04] 时间戳与日期互转
来源：http://uao.9152youxi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rdi.wangshuangyany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pda.hywenlv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mxg.chenjidiqi.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://cmm.yanxiufei.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xyy.jqgfzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uiy.epnwcf.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qia.feifeiyinyue.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eao.jinyuanbaomall.cn

[J05] 时间加减（加 7 天）
来源：http://zkj.9152youxi.cn

Py:   now + timedelta(days=7)
来源：http://wlp.chenzaomai.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://fkk.nanxuanxn.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rqu.shuidangran.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oqq.yueranfly.top

Java: LocalDate.now().plusDays(7)
来源：http://afd.yangfankeji.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zci.yongpay.top

Ruby: Time.now + 7 * 86400
来源：http://axp.hcnkem.com

C#:   DateTime.Now.AddDays(7)
来源：http://vhg.bjfxy.top

[J06] 计算两时间之差
来源：http://wek.yj20258.top

Py:   (end - start).total_seconds()
来源：http://csr.zdqjudy.top

PHP:  $end->diff($start)->days;
来源：http://erl.shanyushiyangtech.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kwp.shanyushiyangkeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yyh.uphjek.com

Java: Duration.between(start, end).toSeconds()
来源：http://wre.xingfuxueyuan.xyz

Go:   end.Sub(start).Hours()
来源：http://uul.zdqjudy.top

Ruby: end - start                 # 返回秒数
来源：http://hld.epnwcf.com

C#:   (end - start).TotalSeconds
来源：http://vrf.dashuyun.cn

[J07] 比较两个日期
来源：http://qac.havefunace.top

Py:   d1 < d2;  d1 == d2
来源：http://nry.tarul.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hoj.yvedp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uzh.nwbrower.top

TS:   d1.getTime() < d2.getTime()
来源：http://txa.vqdsnc.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wfi.daria6918.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hza.guannengcc.top

Ruby: d1 < d2;  d1 == d2
来源：http://tth.jqgfzy.top

C#:   d1 < d2;  d1 == d2
来源：http://drj.ydzc1.top

[J08] 提取年月日与星期
来源：http://gek.zhiwuduotai.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tva.fzhhl.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wsf.316326.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vfd.xuetiantiany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nzv.yangfankeji.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yie.guowangkeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mdo.xylfe.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lib.epnwcf.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zqf.zhijiandao.cn

[J09] 时区处理
来源：http://wnm.cqqwz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://taf.yj20258.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bgx.pengpengdd.cyou

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xbv.gotoacloud.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mur.xingfuxueyuan.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eqy.mhx1999.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qcv.fehbvm.com

Ruby: Time.now.getlocal("+08:00")
来源：http://iax.yuxming.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://coy.pengpengdd.cyou

[J10] 取今天 / 本月第一天
来源：http://tpm.jyoumei.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://grw.havefunace.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jyd.tianlin.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tjl.ywan-chungtsiang.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nug.c1oappe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pob.daria6918.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ubb.guowangkeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://snu.cdnleiting.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oto.xuanzx.com

================================================================================
来源：http://yzh.cucudq.cn

K. JSON 与序列化
来源：http://rnb.hfpthk.cn

================================================================================
来源：http://pwa.hammf.cn

[K01] 对象转 JSON 字符串
来源：http://wrc.bbcook.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tfq.sweek.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cgf.zhaomingkeji.xyz

JS:   JSON.stringify(obj)
来源：http://sya.cashguo.top

TS:   JSON.stringify(obj)
来源：http://pvi.pycfn.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://arq.hnqzz.top

Go:   json.Marshal(obj)
来源：http://iza.gzhubu.top

Ruby: obj.to_json                                     // require "json"
来源：http://rid.uphjek.com

C#:   JsonSerializer.Serialize(obj)
来源：http://trh.shangyingyoupin.top

[K02] JSON 字符串转对象
来源：http://afo.fehbvm.com

Py:   json.loads(s)
来源：http://cvg.yj20258888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yza.sufxvd.cn

JS:   JSON.parse(s)
来源：http://qxk.svipenyu.cn

TS:   JSON.parse(s)
来源：http://rfd.yueranfly.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ret.yuanzhike.top

Go:   json.Unmarshal(data, &v)
来源：http://fkm.wangshuangyany.cn

Ruby: JSON.parse(s)
来源：http://fex.hywenlv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://iip.yanxiufei.cn

[K03] JSON 美化输出（带缩进）
来源：http://hlk.sufxvd.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bmp.quarkkingdee.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pmq.daria6918.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qil.ydjk.org.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xil.yangfankeji.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bxs.xylfe.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lcx.zhiwuduotai.top

Ruby: JSON.pretty_generate(obj)
来源：http://tzo.kuanghao11.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lpd.birdmap.top

[K04] 读取 JSON 文件
来源：http://ajz.9152youxi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zxa.yfazqb.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vyv.bjfxy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kvo.yj202588.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rww.hcnkem.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://buf.yj20258.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ano.zhiwuduotai.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://cef.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ohu.shangyingyoupin.top

[K05] 深拷贝对象
来源：http://djm.yuxming.cn

Py:   copy.deepcopy(obj)
来源：http://rak.xuetiantiany.cn

PHP:  unserialize(serialize($obj));
来源：http://pld.wangdashe.top

JS:   structuredClone(obj)
来源：http://rnc.52xcode.cn

TS:   structuredClone(obj)
来源：http://ccf.ctjpmb.com

Java: // 手写拷贝构造，或序列化往返
来源：http://cob.jqgufenzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://skk.zdbjq.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://iob.yonumen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://xzv.wangshuangyany.cn

[K06] 解析 URL 查询串
来源：http://aqr.9152youxi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yjk.chenjidiqi.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sgy.shzxlz.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vbc.xingfuxueyuan.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mrf.chenjidiqi.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cfj.9152youxi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://geg.tarul.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baq.redwolf501.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lqb.hesvh.cn

[K07] 进制转换
来源：http://qym.yvedp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wjy.yj20258.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fly.xingfuxueyuan.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ifb.xinyue.icu

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jtw.zdqjudy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ixp.sysykeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rso.yuanzhike.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zgl.gotoacloud.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bdo.yj20258888.top

[K08] 二进制序列化（非 JSON）
来源：http://umd.shzxlz.cn

Py:   pickle.dumps(obj)
来源：http://xjf.shanyushiyangtech.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xpn.hfpthk.cn

JS:   v8.serialize(obj)        // Node
来源：http://dhb.fanxiaobao.xyz

TS:   v8.serialize(obj)        // Node
来源：http://ojb.jinqigufen.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dwx.hammf.cn

Go:   encoding/gob
来源：http://lpj.zhijiandao.cn

Ruby: Marshal.dump(obj)
来源：http://hec.xingfuxueyuan.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qvn.hcnkem.com

================================================================================
来源：http://ggf.wangdashe.top

L. 网络请求
来源：http://iam.hfpthk.cn

================================================================================
来源：http://sly.jqgfzy.top

[L01] 发送 GET 请求
来源：http://uwv.shuidangran.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cxi.yj20258888.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ilo.xuetiantiany.cn

JS:   await fetch(url)
来源：http://pjy.zdbjq.cn

TS:   await fetch(url)
来源：http://naf.hfpthk.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://svo.chenzaomai.com

Go:   resp, err := http.Get(url)
来源：http://hsa.jiagoushi.top

Ruby: Net::HTTP.get(URI(url))
来源：http://bxn.wangdashe.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hnn.jianghu66.top

[L02] 发送 POST JSON
来源：http://hxh.ybcxt.top

Py:   requests.post(url, json={"a": 1})
来源：http://udc.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gqz.birdmap.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ydr.havefunace.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hxg.wangshuangyany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://spz.zhaomingkeji.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fij.andypj.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cdt.sjlbkw.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://utw.ydzc1.top

[L03] 设置自定义请求头
来源：http://bhw.sjlbkw.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fjp.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vjx.xingfuxueyuan.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vuw.andypj.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xqu.quarkkingdee.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://imk.9152youxi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ocx.yangfankeji.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pog.xziqi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blz.zdbjq.cn

[L04] 设置超时
来源：http://trs.ctjpmb.com

Py:   requests.get(url, timeout=5)
来源：http://evn.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mcu.shanyushiyangkeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nta.xuetiantiany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bzs.fzhhl.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vkk.zhijiandao.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vmb.yj20258888.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lkv.zycfv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yai.pycfn.com

[L05] 上传文件（multipart）
来源：http://kgf.yongpay.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hhv.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sal.zhongyouzk.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zxr.yanxiufei.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oxj.ywan-chungtsiang.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://syw.jinqigfzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vyb.fzhhl.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jcm.yongpay.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sib.fengsongda.top

[L06] 解析响应为 JSON
来源：http://zbj.xingfuxueyuan.xyz

Py:   resp.json()
来源：http://hsm.gzhubu.top

PHP:  json_decode($body, true);
来源：http://kkj.nanxinkj.top

JS:   await resp.json()
来源：http://sft.xingfuxueyuan.xyz

TS:   await resp.json()
来源：http://yqv.guannengcc.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xfm.ctjpmb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fuc.jinyuanbaomall.cn

Ruby: JSON.parse(resp.body)
来源：http://ppv.uphjek.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vey.hfpthk.cn

[L07] 处理 HTTP 状态码
来源：http://iep.bbcook.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pqa.shanyushiyangkeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ecd.guannengcc.top

JS:   resp.ok;  resp.status
来源：http://vjh.hfpthk.cn

TS:   resp.ok;  resp.status
来源：http://pss.yuanzhike.top

Java: resp.statusCode()
来源：http://bzw.vqdsnc.cn

Go:   resp.StatusCode
来源：http://szm.fzhhl.top

Ruby: resp.code.to_i
来源：http://ogd.nanxinkj.top

C#:   (int)resp.StatusCode
来源：http://hlo.jianghu66.top

[L08] 并发请求多个地址
来源：http://nzw.dianchejie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ucp.gogol.net.cn

PHP:  curl_multi_init() 系列
来源：http://nsx.xinyue.icu

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wif.bjfxy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rdj.316326.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lqi.jianghu66.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mnx.aizwys.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://iuz.pengpengdd.cyou

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://acv.cashguo.top

================================================================================
来源：http://qoh.daria6918.cn

M. 命令行 / 进程 / 环境
来源：http://dul.xinyue.icu

================================================================================
来源：http://org.gogol.net.cn

[M01] 读取命令行参数
来源：http://sum.pengpengdd.cyou

Py:   sys.argv[1:]
来源：http://lhs.sufxvd.cn

PHP:  $argv;  $argc;
来源：http://eex.vehdjk.com


<!-- 参考信息 -->