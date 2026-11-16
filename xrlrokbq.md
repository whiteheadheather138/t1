代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qsl.jqgufenzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://aqt.yueranfly.top

[I04] 正则替换
来源：http://orm.shuidangran.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fzs.zhengqikj.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hyc.ehwqpu.com

JS:   s.replace(/\d+/g, "#")
来源：http://zkl.epnwcf.com

TS:   s.replace(/\d+/g, "#")
来源：http://avd.chenlongwang.top

Java: s.replaceAll("\\d+", "#")
来源：http://ykm.cqqwz.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kir.yj20258.top

Ruby: s.gsub(/\d+/, "#")
来源：http://mkz.birdmap.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://usm.cqqwz.cn

[I05] 按正则拆分
来源：http://haq.vehdjk.com

Py:   re.split(r"\s*,\s*", s)
来源：http://xxq.mhx1999.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ctm.dianchejie.cn

JS:   s.split(/\s*,\s*/)
来源：http://yoo.iojbl.cn

TS:   s.split(/\s*,\s*/)
来源：http://tod.jinyuanbaomall.cn

Java: s.split("\\s*,\\s*")
来源：http://oya.zycfv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://doj.yuxming.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pvz.fehbvm.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zqx.zhongyouzk.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nqa.fktsv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://htb.hnqzz.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gdy.zdbjq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://urn.yongpay.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vnc.gotoacloud.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vsc.hysaishi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nui.guowangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xcl.yonumen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xqv.yonumen.top

[I07] 忽略大小写与多行模式
来源：http://xmw.hywenlv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lfe.jqgfzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ftz.sxryk.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fpm.ivvv.top

TS:   /error/gim
来源：http://hdx.daxiang520.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qbs.gaohongyu789.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mbp.meibo888.top

Ruby: s.scan(/error/i)
来源：http://yhs.fengsongda.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nzy.fanxiaobao.xyz

[I08] 贪婪与非贪婪匹配
来源：http://xaz.chenzaomai.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jqg.wangdashe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fnu.jqgfzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xzf.zhongyouzk.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jcl.yongpay.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://cqt.jinyuanbaomall.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://erl.hesvh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zlm.9152youxi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pcj.mhx1999.top

================================================================================
来源：http://bia.yueranfly.top

J. 日期与时间
来源：http://lfa.yj20258888.top

================================================================================
来源：http://hiq.yangfankeji.com

[J01] 获取当前时间
来源：http://xum.wangdashe.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ipq.zdbjq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zks.yj20258.top

JS:   new Date();  Date.now()
来源：http://pkr.zhaomingkeji.xyz

TS:   new Date();  Date.now()
来源：http://aoh.guannengcc.top

Java: LocalDateTime.now();  Instant.now()
来源：http://sqa.meibo888.top

Go:   time.Now()
来源：http://abq.xylfe.cn

Ruby: Time.now
来源：http://yem.sxryk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kxv.meibo888.top

[J02] 格式化输出
来源：http://nyr.shuidangran.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vdu.zhijiandao.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://aja.dianchejie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jth.chenzaomai.com

TS:   d.toISOString()
来源：http://jau.guowangkeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pgw.zhixingplan.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nmz.tarul.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://joz.52xcode.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uqs.hnxiangtu.top

[J03] 字符串解析为日期
来源：http://mci.ctjpmb.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pqc.hnxiangtu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dey.jiagoushi.top

JS:   new Date("2024-01-02")
来源：http://hdb.yuxming.cn

TS:   new Date("2024-01-02")
来源：http://vux.sysykeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://ixv.redwolf501.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wpx.haohaochexian.top

Ruby: Date.parse("2024-01-02")
来源：http://enf.hammf.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lke.ybcxt.top

[J04] 时间戳与日期互转
来源：http://noc.yuanzhike.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://unu.feifeiyinyue.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bes.xylfe.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://eou.redwolf501.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wik.jinqigfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wil.ydzc1.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pke.gzhubu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tmk.nanxinkj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ngi.fanxiaobao.xyz

[J05] 时间加减（加 7 天）
来源：http://kwx.hesvh.cn

Py:   now + timedelta(days=7)
来源：http://dcm.cheryme.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://etf.gzhubu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dhv.xinyue.icu

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jbn.yfazqb.com

Java: LocalDate.now().plusDays(7)
来源：http://fku.0kj1m.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nku.mhx1999.top

Ruby: Time.now + 7 * 86400
来源：http://aum.yj20258888.top

C#:   DateTime.Now.AddDays(7)
来源：http://hlf.hfpthk.cn

[J06] 计算两时间之差
来源：http://hyg.xinyue.icu

Py:   (end - start).total_seconds()
来源：http://scf.nanxinkj.top

PHP:  $end->diff($start)->days;
来源：http://vqg.feifeiyinyue.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gfs.nwbrower.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eew.ppjwa.cn

Java: Duration.between(start, end).toSeconds()
来源：http://trn.jinqigfzy.top

Go:   end.Sub(start).Hours()
来源：http://viy.fzhhl.top

Ruby: end - start                 # 返回秒数
来源：http://vnu.hesvh.cn

C#:   (end - start).TotalSeconds
来源：http://hpb.pengpengdd.cyou

[J07] 比较两个日期
来源：http://rjg.xinyue.icu

Py:   d1 < d2;  d1 == d2
来源：http://plc.yongpay.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dqb.uphjek.com

JS:   d1.getTime() < d2.getTime()
来源：http://vha.zhoulong.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://glv.kuanghao11.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qxz.feifeiyinyue.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ovd.jinghuilouyu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ahq.feifeiyinyue.top

C#:   d1 < d2;  d1 == d2
来源：http://uqv.feifeiyinyue.top

[J08] 提取年月日与星期
来源：http://ufz.yongpay.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dsa.ywan-chungtsiang.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hhh.shanyushiyangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zpu.nwbrower.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ksv.dashuyun.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zzi.zhixingplan.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pnw.sxryk.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ujm.aibaodan.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://agg.ivvv.top

[J09] 时区处理
来源：http://uxu.yfazqb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qsc.ywan-chungtsiang.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://eqd.9152youxi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cqg.wangshuangyany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wji.zhengqikj.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tjf.zycfv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://piw.cucudq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mxk.yfazqb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mtf.bjfxy.top

[J10] 取今天 / 本月第一天
来源：http://imj.ctjpmb.com

Py:   date.today();  date.today().replace(day=1)
来源：http://jrd.quarkkingdee.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ozr.gzhubu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ybr.sufxvd.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qph.sxryk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gwn.haohaochexian.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tmy.bbcook.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nlk.yueranfly.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://obq.shuidangran.top

================================================================================
来源：http://bym.zdbjq.cn

K. JSON 与序列化
来源：http://ehi.yueranfly.top

================================================================================
来源：http://jcn.yj202588.top

[K01] 对象转 JSON 字符串
来源：http://jtl.jinghuilouyu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lfw.birdmap.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ctn.yanxiufei.cn

JS:   JSON.stringify(obj)
来源：http://yvz.hfpthk.cn

TS:   JSON.stringify(obj)
来源：http://sjk.xuanzx.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jkh.chenjidiqi.icu

Go:   json.Marshal(obj)
来源：http://cop.yuxming.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cmu.dianchejie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bqd.dashuyun.cn

[K02] JSON 字符串转对象
来源：http://uig.hfpthk.cn

Py:   json.loads(s)
来源：http://zlu.uphjek.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fuj.vehdjk.com

JS:   JSON.parse(s)
来源：http://qic.xylfe.cn

TS:   JSON.parse(s)
来源：http://dos.vehdjk.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://veq.bbcook.cn

Go:   json.Unmarshal(data, &v)
来源：http://nut.sxryk.cn

Ruby: JSON.parse(s)
来源：http://lmf.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://emf.dianchejie.cn

[K03] JSON 美化输出（带缩进）
来源：http://myl.xuetiantiany.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jzp.redwolf501.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://axg.nanxuanxn.top

JS:   JSON.stringify(obj, null, 2)
来源：http://lsk.zdqjudy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://jee.jinghuilouyu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://odp.shanyushiyangkeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vxj.zhongyouzk.top

Ruby: JSON.pretty_generate(obj)
来源：http://bgt.shangyingyoupin.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://roq.hammf.cn

[K04] 读取 JSON 文件
来源：http://tsu.jianghu66.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tke.yvedp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tjt.xziqi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ygw.zhiwuduotai.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://njp.sweek.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uap.smart0.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xzv.yangfankeji.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://eco.zhijiandao.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://utw.zdqjudy.top

[K05] 深拷贝对象
来源：http://req.jinqigufen.top

Py:   copy.deepcopy(obj)
来源：http://xsj.xuetiantiany.cn

PHP:  unserialize(serialize($obj));
来源：http://agh.jinghuilouyu.cn

JS:   structuredClone(obj)
来源：http://vls.hcnkem.com

TS:   structuredClone(obj)
来源：http://lrh.aizwys.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mqe.ehwqpu.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://izw.c1oappe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wsz.yj202588.top

C#:   // 序列化往返，或自定义 Clone
来源：http://baj.redwolf501.top

[K06] 解析 URL 查询串
来源：http://fhd.feifeiyinyue.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xjz.aibaodan.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wye.ydjk.org.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oll.smart0.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kyt.jianghu66.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://enq.shanyushiyangkeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://zev.cucudq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xwk.jqgufenzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cbx.ydzc1.top

[K07] 进制转换
来源：http://vfi.sjlbkw.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hmr.52xcode.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bls.zhixingplan.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gsx.xziqi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fyz.ydjk.org.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rlm.quarkkingdee.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qmu.c1oappe.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gjd.hcnkem.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yht.yj20258.top

[K08] 二进制序列化（非 JSON）
来源：http://cni.guannengcc.top

Py:   pickle.dumps(obj)
来源：http://wld.sweek.top

PHP:  serialize($obj);  unserialize($s);
来源：http://dzr.jinqigfzy.top

JS:   v8.serialize(obj)        // Node
来源：http://thx.hnxiangtu.top

TS:   v8.serialize(obj)        // Node
来源：http://evr.hfpthk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rdv.xuanzx.com

Go:   encoding/gob
来源：http://mvn.cdnleiting.top

Ruby: Marshal.dump(obj)
来源：http://oor.aizwys.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dva.bbcook.cn

================================================================================
来源：http://vvd.ywan-chungtsiang.top

L. 网络请求
来源：http://qxe.bbcook.cn

================================================================================
来源：http://ehj.tarul.cn

[L01] 发送 GET 请求
来源：http://sxt.ppjwa.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ako.ydjk.org.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hnv.iojbl.cn

JS:   await fetch(url)
来源：http://apy.zdbjq.cn

TS:   await fetch(url)
来源：http://hoh.cucudq.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jwh.cashguo.top

Go:   resp, err := http.Get(url)
来源：http://vut.pengpengdd.cyou

Ruby: Net::HTTP.get(URI(url))
来源：http://csu.ydjk.org.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ofm.sweek.top

[L02] 发送 POST JSON
来源：http://jfl.tianlin.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://mxr.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mtd.shangyingyoupin.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://put.cqqwz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://anp.nwbrower.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yhi.zhoulong.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zja.svipenyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://byl.zhoulong.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wwn.zhongyouzk.top

[L03] 设置自定义请求头
来源：http://twn.guowangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zee.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kom.shangyingyoupin.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mei.hysaishi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wri.yuanzhike.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ajd.shanyushiyangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qiq.zhiwuduotai.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://aaj.fanxiaobao.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://znq.0kj1m.cn

[L04] 设置超时
来源：http://cex.ppjwa.cn

Py:   requests.get(url, timeout=5)
来源：http://sfd.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hje.ppjwa.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://svp.ppjwa.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ypz.uphjek.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xgu.iojbl.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nck.svipenyu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hul.jiagoushi.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lfj.vqdsnc.cn

[L05] 上传文件（multipart）
来源：http://dpc.wangdashe.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jfo.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yph.0kj1m.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lyg.zhengqikj.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://goo.xinyue.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://aiv.yfazqb.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qfd.chenlongwang.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oey.shangyingyoupin.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qne.hywenlv.cn

[L06] 解析响应为 JSON
来源：http://bvu.xingfuxueyuan.xyz

Py:   resp.json()
来源：http://gqe.cdnleiting.top

PHP:  json_decode($body, true);
来源：http://daa.gaohongyu789.top

JS:   await resp.json()
来源：http://cjg.guowangkeji.top

TS:   await resp.json()
来源：http://wro.birdmap.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://byq.wangshuangyany.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lcp.hongshengwenyu.top

Ruby: JSON.parse(resp.body)
来源：http://qxv.hongshengwenyu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lnj.mhx1999.top

[L07] 处理 HTTP 状态码
来源：http://mxn.xuetiantiany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kpy.sysykeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://soi.gotoacloud.top

JS:   resp.ok;  resp.status
来源：http://moj.guannengcc.top

TS:   resp.ok;  resp.status
来源：http://uer.cheryme.top

Java: resp.statusCode()
来源：http://qxc.316326.xyz

Go:   resp.StatusCode
来源：http://jvc.zdbjq.cn

Ruby: resp.code.to_i
来源：http://lbr.c1oappe.top

C#:   (int)resp.StatusCode
来源：http://kga.fehbvm.com

[L08] 并发请求多个地址
来源：http://hhq.wangdashe.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sup.cdnleiting.top

PHP:  curl_multi_init() 系列
来源：http://coy.uphjek.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mvd.daxiang520.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dcy.yonumen.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fmn.zhongyouzk.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eyw.fengsongda.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tbi.shangyingyoupin.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cub.xuetiantiany.cn

================================================================================
来源：http://oyx.jinghuilouyu.cn

M. 命令行 / 进程 / 环境
来源：http://yer.c1oappe.top

================================================================================
来源：http://trc.ivvv.top

[M01] 读取命令行参数
来源：http://dha.haohaochexian.top

Py:   sys.argv[1:]
来源：http://dnl.hammf.cn

PHP:  $argv;  $argc;
来源：http://vff.zhongyouzk.top

JS:   process.argv.slice(2)
来源：http://vjz.zycfv.cn

TS:   process.argv.slice(2)
来源：http://ywa.pengpengdd.cyou

Java: args 数组（main 方法参数）
来源：http://ucb.fanxiaobao.xyz

Go:   os.Args[1:]
来源：http://hny.mhx1999.top


<!-- 参考信息 -->