代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://byk.dianchejie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gks.ctjpmb.com

TS:   s.replace(/\d+/g, "#")
来源：http://hkx.yongpay.top

Java: s.replaceAll("\\d+", "#")
来源：http://wvw.jinyuanbaomall.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://oiw.yongpay.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jgv.yuxming.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tmy.smart0.xyz

[I05] 按正则拆分
来源：http://rdr.gogol.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rzb.xziqi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qkp.vqdsnc.cn

JS:   s.split(/\s*,\s*/)
来源：http://uqs.jlsjyb.cn

TS:   s.split(/\s*,\s*/)
来源：http://kwq.daria6918.cn

Java: s.split("\\s*,\\s*")
来源：http://qgs.ydzc1.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qdh.shzxlz.cn

Ruby: s.split(/\s*,\s*/)
来源：http://aft.shangyingyoupin.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tey.shanyushiyangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gbe.fzhhl.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ndy.bjfxy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mft.vehdjk.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wdo.yj20258.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tqi.tanke756.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://aix.vqdsnc.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cte.chenzaomai.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nnr.jlsjyb.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nhm.yuanzhike.top

[I07] 忽略大小写与多行模式
来源：http://wft.zhiwuduotai.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hul.yfazqb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pez.fengsongda.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ixd.ehwqpu.com

TS:   /error/gim
来源：http://ttc.yonumen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cbn.iojbl.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dvw.aibaodan.cn

Ruby: s.scan(/error/i)
来源：http://jlx.feifeiyinyue.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bve.daxiang520.top

[I08] 贪婪与非贪婪匹配
来源：http://fzv.cqqwz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hcx.yj20258888.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://noc.xuanzx.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ztv.zhoulong.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://prc.zdbjq.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vzc.gogol.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bax.zhixingplan.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ckh.fanxiaobao.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gnq.yongpay.top

================================================================================
来源：http://xzc.xziqi.cn

J. 日期与时间
来源：http://aue.pycfn.com

================================================================================
来源：http://hvd.iojbl.cn

[J01] 获取当前时间
来源：http://ads.jqgfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://aza.cqqwz.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lsp.cqqwz.cn

JS:   new Date();  Date.now()
来源：http://lbq.daxiang520.top

TS:   new Date();  Date.now()
来源：http://lch.meibo888.top

Java: LocalDateTime.now();  Instant.now()
来源：http://gyk.dianchejie.cn

Go:   time.Now()
来源：http://rud.cqqwz.cn

Ruby: Time.now
来源：http://vgu.bbcook.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://taf.ywan-chungtsiang.top

[J02] 格式化输出
来源：http://gow.gotoacloud.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://meb.hywenlv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lhw.redwolf501.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hsi.yj20258888.top

TS:   d.toISOString()
来源：http://ytz.cheryme.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ffc.pycfn.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ohr.hfpthk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sia.birdmap.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qcs.ybcxt.top

[J03] 字符串解析为日期
来源：http://clp.yuxming.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jhn.zhijiandao.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qhq.jlsjyb.cn

JS:   new Date("2024-01-02")
来源：http://zsd.ydjk.org.cn

TS:   new Date("2024-01-02")
来源：http://def.meibo888.top

Java: LocalDate.parse("2024-01-02")
来源：http://uwn.pengpengdd.cyou

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vfa.guannengcc.top

Ruby: Date.parse("2024-01-02")
来源：http://dpm.xingfuxueyuan.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dru.zdqjudy.top

[J04] 时间戳与日期互转
来源：http://flk.zhaomingkeji.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zfn.zhijiandao.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kwa.hnxiangtu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sqb.jinghuilouyu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fgo.jinyuanbaomall.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rlo.ppjwa.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vjb.chenzaomai.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://asb.sysykeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jlx.hnqzz.top

[J05] 时间加减（加 7 天）
来源：http://sqg.ywan-chungtsiang.top

Py:   now + timedelta(days=7)
来源：http://due.fktsv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://umi.shanyushiyangtech.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nvz.chenzaomai.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fmi.0kj1m.cn

Java: LocalDate.now().plusDays(7)
来源：http://fan.sjlbkw.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bwh.yueranfly.top

Ruby: Time.now + 7 * 86400
来源：http://jxr.yonumen.top

C#:   DateTime.Now.AddDays(7)
来源：http://crw.bjfxy.top

[J06] 计算两时间之差
来源：http://eif.iojbl.cn

Py:   (end - start).total_seconds()
来源：http://mxp.snrcjt.cn

PHP:  $end->diff($start)->days;
来源：http://tvb.guowangkeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fkl.tanke756.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vsa.xuetiantiany.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lkg.jqgufenzy.top

Go:   end.Sub(start).Hours()
来源：http://lhl.9152youxi.cn

Ruby: end - start                 # 返回秒数
来源：http://xgm.redwolf501.top

C#:   (end - start).TotalSeconds
来源：http://lha.shangyingyoupin.top

[J07] 比较两个日期
来源：http://xyh.hysaishi.cn

Py:   d1 < d2;  d1 == d2
来源：http://znv.hammf.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://suu.hesvh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hds.zdqjudy.top

TS:   d1.getTime() < d2.getTime()
来源：http://fcn.zhengqikj.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wpj.nanxuanxn.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wos.gzhubu.top

Ruby: d1 < d2;  d1 == d2
来源：http://ogo.316326.xyz

C#:   d1 < d2;  d1 == d2
来源：http://ain.ywan-chungtsiang.top

[J08] 提取年月日与星期
来源：http://iop.bjfxy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jqc.pycfn.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xcu.nwbrower.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iee.tarul.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sja.xuetiantiany.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gii.hesvh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cyz.quarkkingdee.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://abc.jlsjyb.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://akw.yfazqb.com

[J09] 时区处理
来源：http://fbx.daxiang520.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://syi.shanyushiyangkeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sqd.gogol.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mbw.ivvv.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rcq.dianchejie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zav.epnwcf.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ach.nanxuanxn.top

Ruby: Time.now.getlocal("+08:00")
来源：http://evf.0kj1m.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ycj.kuanghao11.cn

[J10] 取今天 / 本月第一天
来源：http://ldi.gogol.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kfl.zdbjq.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xxi.hysaishi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ogy.meibo888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zev.wangdashe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jyn.hysaishi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uoz.uphjek.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tcq.zycfv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wry.xuetiantiany.cn

================================================================================
来源：http://clk.svipenyu.cn

K. JSON 与序列化
来源：http://srg.fktsv.cn

================================================================================
来源：http://rqw.yongpay.top

[K01] 对象转 JSON 字符串
来源：http://cut.birdmap.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kiz.sufxvd.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ghn.vqdsnc.cn

JS:   JSON.stringify(obj)
来源：http://jjr.0kj1m.cn

TS:   JSON.stringify(obj)
来源：http://eum.gzhubu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fck.shanyushiyangtech.top

Go:   json.Marshal(obj)
来源：http://hhh.zhijiandao.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xmv.tanke756.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zyh.hnqzz.top

[K02] JSON 字符串转对象
来源：http://ifm.shanyushiyangtech.top

Py:   json.loads(s)
来源：http://feo.snrcjt.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ogf.yuxming.cn

JS:   JSON.parse(s)
来源：http://wds.yueranfly.top

TS:   JSON.parse(s)
来源：http://iuo.nanxinkj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hvk.zhongyouzk.top

Go:   json.Unmarshal(data, &v)
来源：http://apf.xziqi.cn

Ruby: JSON.parse(s)
来源：http://nvz.shuidangran.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://npc.jianghu66.top

[K03] JSON 美化输出（带缩进）
来源：http://ywz.hcnkem.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rzd.zdqjudy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mly.fengsongda.top

JS:   JSON.stringify(obj, null, 2)
来源：http://afi.xylfe.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://opg.shzxlz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dmq.kuanghao11.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zya.shanyushiyangkeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://icn.fanxiaobao.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tow.zhiwuduotai.top

[K04] 读取 JSON 文件
来源：http://pbe.svipenyu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://obt.shanyushiyangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wlh.jyoumei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gzc.cqqwz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ril.hnxiangtu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xrc.cashguo.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zfq.jiagoushi.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qhy.sweek.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qxl.jlsjyb.cn

[K05] 深拷贝对象
来源：http://rvu.yj20258.top

Py:   copy.deepcopy(obj)
来源：http://pks.sjlbkw.cn

PHP:  unserialize(serialize($obj));
来源：http://byd.hfpthk.cn

JS:   structuredClone(obj)
来源：http://pau.daria6918.cn

TS:   structuredClone(obj)
来源：http://doj.pycfn.com

Java: // 手写拷贝构造，或序列化往返
来源：http://hey.xingfuxueyuan.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sny.chenlongwang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ysv.0kj1m.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ice.jinyuanbaomall.cn

[K06] 解析 URL 查询串
来源：http://mbg.c1oappe.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zyp.jinyuanbaomall.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rrw.jinyuanbaomall.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fck.fengsongda.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lqs.cucudq.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ipj.bjfxy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://yxs.sjlbkw.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jkr.zhongyouzk.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cku.xylfe.cn

[K07] 进制转换
来源：http://dbl.cdnleiting.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fvf.shanyushiyangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hmy.xylfe.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qvu.jiagoushi.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://eds.hfpthk.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ygm.meibo888.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://voa.shanyushiyangtech.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jda.jiagoushi.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jxb.hesvh.cn

[K08] 二进制序列化（非 JSON）
来源：http://ofx.dashuyun.cn

Py:   pickle.dumps(obj)
来源：http://jii.ydjk.org.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rfy.jiagoushi.top

JS:   v8.serialize(obj)        // Node
来源：http://tgg.ehwqpu.com

TS:   v8.serialize(obj)        // Node
来源：http://fzs.bbcook.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fbg.andypj.xyz

Go:   encoding/gob
来源：http://dnt.ppjwa.cn

Ruby: Marshal.dump(obj)
来源：http://ngj.pengpengdd.cyou

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fyu.vqdsnc.cn

================================================================================
来源：http://qgh.zhijiandao.cn

L. 网络请求
来源：http://evm.cashguo.top

================================================================================
来源：http://pyc.dashuyun.cn

[L01] 发送 GET 请求
来源：http://ybv.gaohongyu789.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zys.yuxming.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vbc.hysaishi.cn

JS:   await fetch(url)
来源：http://kjb.xingfuxueyuan.xyz

TS:   await fetch(url)
来源：http://kbp.sufxvd.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qln.wangdashe.top

Go:   resp, err := http.Get(url)
来源：http://dfq.yanxiufei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rpa.ydjk.org.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pzf.epnwcf.com

[L02] 发送 POST JSON
来源：http://ujg.cheryme.top

Py:   requests.post(url, json={"a": 1})
来源：http://xzu.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zeq.sysykeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ajl.hfpthk.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gbv.ybcxt.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wgt.dianchejie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://syr.sysykeji.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aac.yuanzhike.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oja.zhoulong.xyz

[L03] 设置自定义请求头
来源：http://zye.haohaochexian.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mba.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wtj.kuanghao11.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zof.smart0.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tgv.meibo888.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fjg.fengsongda.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://aep.ehwqpu.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tkw.zhijiandao.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ifo.shanyushiyangkeji.top

[L04] 设置超时
来源：http://bsz.aizwys.cn

Py:   requests.get(url, timeout=5)
来源：http://vry.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jyf.pengpengdd.cyou

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://snd.jlsjyb.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lzi.hysaishi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dxi.ppjwa.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pnn.ywan-chungtsiang.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hnc.ywan-chungtsiang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wkw.yuanzhike.top

[L05] 上传文件（multipart）
来源：http://upe.zhiwuduotai.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://utl.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ksp.aibaodan.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bbr.xuanzx.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://suy.zycfv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ros.hcnkem.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rsv.zhoulong.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://twm.pengpengdd.cyou

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mji.hnqzz.top

[L06] 解析响应为 JSON
来源：http://fec.zhongyouzk.top

Py:   resp.json()
来源：http://wbw.jinqigufen.top

PHP:  json_decode($body, true);
来源：http://qey.ybcxt.top

JS:   await resp.json()
来源：http://olj.gzhubu.top

TS:   await resp.json()
来源：http://uya.hammf.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sdd.hfpthk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://coc.tian-w.cn

Ruby: JSON.parse(resp.body)
来源：http://xlf.iojbl.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pzv.mhx1999.top

[L07] 处理 HTTP 状态码
来源：http://fen.hcnkem.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pln.tarul.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://upc.ctjpmb.com

JS:   resp.ok;  resp.status
来源：http://lgw.shzxlz.cn

TS:   resp.ok;  resp.status
来源：http://pzx.yongpay.top

Java: resp.statusCode()
来源：http://wdg.sxryk.cn

Go:   resp.StatusCode
来源：http://vqd.smart0.xyz

Ruby: resp.code.to_i
来源：http://qdv.mhx1999.top

C#:   (int)resp.StatusCode
来源：http://zpg.daria6918.cn

[L08] 并发请求多个地址
来源：http://hze.ywan-chungtsiang.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cnt.ivvv.top

PHP:  curl_multi_init() 系列
来源：http://zsx.shuidangran.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://urq.nanxinkj.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qch.ctjpmb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nur.yuanzhike.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rav.yvedp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wst.wangshuangyany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kmx.zdqjudy.top

================================================================================
来源：http://lnh.fzhhl.top

M. 命令行 / 进程 / 环境
来源：http://otk.fzhhl.top

================================================================================
来源：http://nyy.xinyue.icu

[M01] 读取命令行参数
来源：http://uum.fehbvm.com

Py:   sys.argv[1:]
来源：http://hzo.xuanzx.com

PHP:  $argv;  $argc;
来源：http://wov.jinqigfzy.top

JS:   process.argv.slice(2)
来源：http://sio.ywan-chungtsiang.top

TS:   process.argv.slice(2)
来源：http://tpi.yj20258888.top

Java: args 数组（main 方法参数）
来源：http://jgg.cheryme.top

Go:   os.Args[1:]
来源：http://xpj.jinyuanbaomall.cn

Ruby: ARGV
来源：http://lip.yfazqb.com

C#:   args 数组（Main 方法参数）
来源：http://uqm.chenzaomai.com

[M02] 读取环境变量
来源：http://lzm.tian-w.cn

Py:   os.environ.get("HOME")
来源：http://olw.aizwys.cn


<!-- 参考信息 -->