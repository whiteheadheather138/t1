代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dno.zhijiandao.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qvn.zhiwuduotai.top

TS:   s.replace(/\d+/g, "#")
来源：http://pgd.zhijiandao.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ooo.yuxming.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jqc.pycfn.com

Ruby: s.gsub(/\d+/, "#")
来源：http://ckm.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://btx.daxiang520.top

[I05] 按正则拆分
来源：http://kxy.chenzaomai.com

Py:   re.split(r"\s*,\s*", s)
来源：http://xig.yuanzhike.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yoz.fzhhl.top

JS:   s.split(/\s*,\s*/)
来源：http://dtb.jinghuilouyu.cn

TS:   s.split(/\s*,\s*/)
来源：http://hhp.jqgufenzy.top

Java: s.split("\\s*,\\s*")
来源：http://mds.zhixingplan.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://spd.shuidangran.top

Ruby: s.split(/\s*,\s*/)
来源：http://bjd.fengsongda.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ujo.hywenlv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tpt.hesvh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ybc.wangdashe.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hbn.hammf.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://luu.hysaishi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cni.0kj1m.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://myo.yuanzhike.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xcf.shzxlz.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ufz.zdbjq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lag.ydzc1.top

[I07] 忽略大小写与多行模式
来源：http://scc.cheryme.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ngw.wangshuangyany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://obs.zhengqikj.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vwg.yanxiufei.cn

TS:   /error/gim
来源：http://rxt.svipenyu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wxt.gotoacloud.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nbv.zycfv.cn

Ruby: s.scan(/error/i)
来源：http://xck.jlsjyb.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nyv.ehwqpu.com

[I08] 贪婪与非贪婪匹配
来源：http://gyz.ywan-chungtsiang.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iqv.yfazqb.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://eeb.uphjek.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://swo.zdbjq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://plv.zdqjudy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://znw.sxryk.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://let.wangshuangyany.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://euv.hammf.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://maj.yanxiufei.cn

================================================================================
来源：http://kfi.hongshengwenyu.top

J. 日期与时间
来源：http://bwd.yueranfly.top

================================================================================
来源：http://bba.yj20258.top

[J01] 获取当前时间
来源：http://ibs.sysykeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://tbd.hnxiangtu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rtp.sweek.top

JS:   new Date();  Date.now()
来源：http://rzv.zhaomingkeji.xyz

TS:   new Date();  Date.now()
来源：http://ebq.cashguo.top

Java: LocalDateTime.now();  Instant.now()
来源：http://noe.hammf.cn

Go:   time.Now()
来源：http://wqd.zhaomingkeji.xyz

Ruby: Time.now
来源：http://nzq.andypj.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://svq.fktsv.cn

[J02] 格式化输出
来源：http://uaz.tarul.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eay.iojbl.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cfw.wangshuangyany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ryv.ybcxt.top

TS:   d.toISOString()
来源：http://xdg.hesvh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gmw.jinghuilouyu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jhq.jqgufenzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://haa.fanxiaobao.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dcr.aibaodan.cn

[J03] 字符串解析为日期
来源：http://hby.zhongyouzk.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ygv.gogol.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://erj.gzhubu.top

JS:   new Date("2024-01-02")
来源：http://nzt.jinqigfzy.top

TS:   new Date("2024-01-02")
来源：http://wai.nwbrower.top

Java: LocalDate.parse("2024-01-02")
来源：http://icx.vqdsnc.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ysn.haohaochexian.top

Ruby: Date.parse("2024-01-02")
来源：http://zqs.hysaishi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bux.havefunace.top

[J04] 时间戳与日期互转
来源：http://etk.chenlongwang.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zur.birdmap.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dma.jlsjyb.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ofm.guowangkeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ydq.bbcook.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jkr.xingfuxueyuan.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zfc.dianchejie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://car.kuanghao11.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ftu.bjfxy.top

[J05] 时间加减（加 7 天）
来源：http://vkk.shzxlz.cn

Py:   now + timedelta(days=7)
来源：http://gsj.epnwcf.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://ctc.pycfn.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oiy.ehwqpu.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://twv.yonumen.top

Java: LocalDate.now().plusDays(7)
来源：http://neu.ydjk.org.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xxq.haohaochexian.top

Ruby: Time.now + 7 * 86400
来源：http://zhk.cqqwz.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mos.vehdjk.com

[J06] 计算两时间之差
来源：http://zxm.yueranfly.top

Py:   (end - start).total_seconds()
来源：http://xsd.birdmap.top

PHP:  $end->diff($start)->days;
来源：http://oew.jyoumei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://aly.dashuyun.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tmw.52xcode.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ehv.yangfankeji.com

Go:   end.Sub(start).Hours()
来源：http://mbi.jinghuilouyu.cn

Ruby: end - start                 # 返回秒数
来源：http://iva.dashuyun.cn

C#:   (end - start).TotalSeconds
来源：http://ytg.xziqi.cn

[J07] 比较两个日期
来源：http://byo.nanxinkj.top

Py:   d1 < d2;  d1 == d2
来源：http://gly.cucudq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ygd.xinyue.icu

JS:   d1.getTime() < d2.getTime()
来源：http://jgm.tarul.cn

TS:   d1.getTime() < d2.getTime()
来源：http://icb.gogol.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://asr.jinqigfzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tdv.redwolf501.top

Ruby: d1 < d2;  d1 == d2
来源：http://yud.zhengqikj.top

C#:   d1 < d2;  d1 == d2
来源：http://vlr.gotoacloud.top

[J08] 提取年月日与星期
来源：http://top.xylfe.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fjc.quarkkingdee.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dbj.chenzaomai.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vjm.hesvh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bum.uphjek.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qmq.zhaomingkeji.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jvb.cheryme.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hzl.zhiwuduotai.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rid.zhongyouzk.top

[J09] 时区处理
来源：http://nel.daria6918.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kvy.zhixingplan.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cuv.sxryk.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pss.wangshuangyany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fdp.cashguo.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nwr.cdnleiting.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zyp.cdnleiting.top

Ruby: Time.now.getlocal("+08:00")
来源：http://lbh.yangfankeji.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lgr.tianlin.xyz

[J10] 取今天 / 本月第一天
来源：http://fzs.bbcook.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kir.chenlongwang.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jvo.jinyuanbaomall.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zch.dashuyun.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oia.gogol.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sdk.mhx1999.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mto.meibo888.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zyf.yj20258888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yeb.meibo888.top

================================================================================
来源：http://uop.haohaochexian.top

K. JSON 与序列化
来源：http://qqh.jinyuanbaomall.cn

================================================================================
来源：http://ezp.jianghu66.top

[K01] 对象转 JSON 字符串
来源：http://wtb.wangdashe.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rvt.gzhubu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bpp.haohaochexian.top

JS:   JSON.stringify(obj)
来源：http://cuz.zhongyouzk.top

TS:   JSON.stringify(obj)
来源：http://kwq.xinyue.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nnk.shanyushiyangtech.top

Go:   json.Marshal(obj)
来源：http://nfg.sufxvd.cn

Ruby: obj.to_json                                     // require "json"
来源：http://anl.daxiang520.top

C#:   JsonSerializer.Serialize(obj)
来源：http://lzo.iojbl.cn

[K02] JSON 字符串转对象
来源：http://uxz.bbcook.cn

Py:   json.loads(s)
来源：http://bds.zdqjudy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yed.fengsongda.top

JS:   JSON.parse(s)
来源：http://jfa.xuanzx.com

TS:   JSON.parse(s)
来源：http://egl.jinqigfzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://aew.bjfxy.top

Go:   json.Unmarshal(data, &v)
来源：http://dnh.yueranfly.top

Ruby: JSON.parse(s)
来源：http://zzl.yongpay.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://obv.0kj1m.cn

[K03] JSON 美化输出（带缩进）
来源：http://xyg.yangfankeji.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oop.daria6918.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nsu.shuidangran.top

JS:   JSON.stringify(obj, null, 2)
来源：http://eas.gzhubu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://abv.ppjwa.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gtk.ehwqpu.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://acy.hysaishi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://guy.hcnkem.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jjb.aizwys.cn

[K04] 读取 JSON 文件
来源：http://hjw.uphjek.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xui.ctjpmb.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://izv.xziqi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://agc.zhaomingkeji.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://knd.ydjk.org.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kay.fktsv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nrm.fktsv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rwz.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kek.nwbrower.top

[K05] 深拷贝对象
来源：http://sbc.zhoulong.xyz

Py:   copy.deepcopy(obj)
来源：http://trm.jinqigfzy.top

PHP:  unserialize(serialize($obj));
来源：http://fvq.ydzc1.top

JS:   structuredClone(obj)
来源：http://bam.hammf.cn

TS:   structuredClone(obj)
来源：http://xjx.gotoacloud.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jfs.tian-w.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wad.xingfuxueyuan.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wok.yj20258.top

C#:   // 序列化往返，或自定义 Clone
来源：http://eud.yuanzhike.top

[K06] 解析 URL 查询串
来源：http://xsy.jianghu66.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://skj.sysykeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tmf.cucudq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ryh.meibo888.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sne.fanxiaobao.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kpi.tianlin.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://hiz.yj20258888.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://snd.zdbjq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xkt.hongshengwenyu.top

[K07] 进制转换
来源：http://syl.shzxlz.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lbg.sweek.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ndl.haohaochexian.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uth.fehbvm.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kvs.316326.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rzf.hnqzz.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cby.sufxvd.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nig.c1oappe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fbu.uphjek.com

[K08] 二进制序列化（非 JSON）
来源：http://gfv.hesvh.cn

Py:   pickle.dumps(obj)
来源：http://dha.hnxiangtu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ouk.daria6918.cn

JS:   v8.serialize(obj)        // Node
来源：http://uvs.xinyue.icu

TS:   v8.serialize(obj)        // Node
来源：http://smc.hammf.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://iej.andypj.xyz

Go:   encoding/gob
来源：http://flo.bbcook.cn

Ruby: Marshal.dump(obj)
来源：http://iks.zhongyouzk.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lun.sysykeji.top

================================================================================
来源：http://nng.yongpay.top

L. 网络请求
来源：http://mjy.yj20258.top

================================================================================
来源：http://viq.bbcook.cn

[L01] 发送 GET 请求
来源：http://hnx.wangdashe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qnl.9152youxi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cct.ybcxt.top

JS:   await fetch(url)
来源：http://tvs.zhaomingkeji.xyz

TS:   await fetch(url)
来源：http://bar.fzhhl.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vvn.hysaishi.cn

Go:   resp, err := http.Get(url)
来源：http://spg.svipenyu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hrg.gzhubu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eih.birdmap.top

[L02] 发送 POST JSON
来源：http://xqv.yonumen.top

Py:   requests.post(url, json={"a": 1})
来源：http://dbw.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://owl.shanyushiyangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pdj.sufxvd.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://onh.jianghu66.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xtm.xuanzx.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sqg.kuanghao11.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xhc.jinqigufen.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mkz.fzhhl.top

[L03] 设置自定义请求头
来源：http://pem.tarul.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yrc.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://idz.zdbjq.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cwn.hcnkem.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zvc.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qrd.ivvv.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pth.xingfuxueyuan.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bdn.kuanghao11.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iqk.quarkkingdee.top

[L04] 设置超时
来源：http://ypi.0kj1m.cn

Py:   requests.get(url, timeout=5)
来源：http://yld.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dgg.uphjek.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vyt.yuxming.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mfw.yangfankeji.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://djz.meibo888.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://miy.bjfxy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hwc.dashuyun.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wpi.gogol.net.cn

[L05] 上传文件（multipart）
来源：http://nxw.meibo888.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kup.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oaj.yanxiufei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gxw.yanxiufei.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ptt.shanyushiyangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ewo.ywan-chungtsiang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ruz.snrcjt.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://piv.xuetiantiany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pan.jlsjyb.cn

[L06] 解析响应为 JSON
来源：http://siz.hfpthk.cn

Py:   resp.json()
来源：http://mpm.chenjidiqi.icu

PHP:  json_decode($body, true);
来源：http://qrt.quarkkingdee.top

JS:   await resp.json()
来源：http://cns.yuanzhike.top

TS:   await resp.json()
来源：http://sxe.guannengcc.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oks.hammf.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jli.xingfuxueyuan.xyz

Ruby: JSON.parse(resp.body)
来源：http://npn.dianchejie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://amp.9152youxi.cn

[L07] 处理 HTTP 状态码
来源：http://qbl.sxryk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kxr.zhoulong.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cid.9152youxi.cn

JS:   resp.ok;  resp.status
来源：http://ceo.cqqwz.cn

TS:   resp.ok;  resp.status
来源：http://yic.hcnkem.com

Java: resp.statusCode()
来源：http://zwk.xuetiantiany.cn

Go:   resp.StatusCode
来源：http://dtw.yj202588.top

Ruby: resp.code.to_i
来源：http://kse.dashuyun.cn

C#:   (int)resp.StatusCode
来源：http://mhu.yueranfly.top

[L08] 并发请求多个地址
来源：http://bzj.zdbjq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wdo.daria6918.cn

PHP:  curl_multi_init() 系列
来源：http://woz.xylfe.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hff.cqqwz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://emw.zdqjudy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kuy.kuanghao11.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ssc.svipenyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tml.zhijiandao.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ttx.hcnkem.com

================================================================================
来源：http://spq.dianchejie.cn

M. 命令行 / 进程 / 环境
来源：http://hqa.ywan-chungtsiang.top

================================================================================
来源：http://hpc.zhengqikj.top

[M01] 读取命令行参数
来源：http://xfe.bjfxy.top

Py:   sys.argv[1:]
来源：http://qah.fzhhl.top

PHP:  $argv;  $argc;
来源：http://kvu.hammf.cn

JS:   process.argv.slice(2)
来源：http://ran.jyoumei.cn

TS:   process.argv.slice(2)
来源：http://fwm.jiagoushi.top

Java: args 数组（main 方法参数）
来源：http://kru.yangfankeji.com

Go:   os.Args[1:]
来源：http://aki.xuetiantiany.cn

Ruby: ARGV
来源：http://cux.nanxuanxn.top

C#:   args 数组（Main 方法参数）
来源：http://biq.hnqzz.top

[M02] 读取环境变量
来源：http://yxl.mhx1999.top

Py:   os.environ.get("HOME")
来源：http://ugc.zhijiandao.cn


<!-- 参考信息 -->