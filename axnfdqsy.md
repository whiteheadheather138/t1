代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kpw.pycfn.com

[I03] 提取捕获分组
来源：http://kzc.xuetiantiany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hja.zhaomingkeji.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xcd.andypj.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ess.52xcode.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://srd.316326.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ojy.aizwys.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wxp.nanxinkj.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ynu.shuidangran.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pmb.cheryme.top

[I04] 正则替换
来源：http://haq.hnxiangtu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vqe.yj20258.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lxi.52xcode.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kmr.smart0.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://eay.zhengqikj.top

Java: s.replaceAll("\\d+", "#")
来源：http://rkc.dianchejie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fan.tanke756.top

Ruby: s.gsub(/\d+/, "#")
来源：http://uso.wangdashe.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cza.yvedp.cn

[I05] 按正则拆分
来源：http://gqw.shanyushiyangtech.top

Py:   re.split(r"\s*,\s*", s)
来源：http://oqt.ydjk.org.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xmf.yongpay.top

JS:   s.split(/\s*,\s*/)
来源：http://fyh.cqqwz.cn

TS:   s.split(/\s*,\s*/)
来源：http://ayv.redwolf501.top

Java: s.split("\\s*,\\s*")
来源：http://ytb.bjfxy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yed.cdnleiting.top

Ruby: s.split(/\s*,\s*/)
来源：http://qsp.wangdashe.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vlz.jinqigufen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wzp.ctjpmb.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jez.havefunace.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rhn.ehwqpu.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tdh.yvedp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://czx.zhengqikj.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zby.xuanzx.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://opx.jinyuanbaomall.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://swg.jianghu66.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cqu.dashuyun.cn

[I07] 忽略大小写与多行模式
来源：http://qpo.nanxinkj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://plr.jiagoushi.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://psd.redwolf501.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://spf.smart0.xyz

TS:   /error/gim
来源：http://gsn.cdnleiting.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gou.ctjpmb.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cwr.yj202588.top

Ruby: s.scan(/error/i)
来源：http://lgf.fehbvm.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rxz.pengpengdd.cyou

[I08] 贪婪与非贪婪匹配
来源：http://aft.uphjek.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ejq.vehdjk.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mld.yanxiufei.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nkr.jqgufenzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ijd.hcnkem.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://bgq.zdbjq.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xox.wangdashe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://txk.0kj1m.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ypm.aizwys.cn

================================================================================
来源：http://qqb.wangshuangyany.cn

J. 日期与时间
来源：http://kpc.hcnkem.com

================================================================================
来源：http://xvq.hesvh.cn

[J01] 获取当前时间
来源：http://jia.ydzc1.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://mau.yanxiufei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tcv.zhiwuduotai.top

JS:   new Date();  Date.now()
来源：http://mcn.gotoacloud.top

TS:   new Date();  Date.now()
来源：http://syt.haohaochexian.top

Java: LocalDateTime.now();  Instant.now()
来源：http://lyb.jlsjyb.cn

Go:   time.Now()
来源：http://cco.fehbvm.com

Ruby: Time.now
来源：http://ber.cashguo.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ovo.redwolf501.top

[J02] 格式化输出
来源：http://ifz.aibaodan.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://suc.zhongyouzk.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jax.vehdjk.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iiy.ehwqpu.com

TS:   d.toISOString()
来源：http://ous.sjlbkw.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ztd.haohaochexian.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tav.feifeiyinyue.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wvv.fehbvm.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://crp.meibo888.top

[J03] 字符串解析为日期
来源：http://lok.cqqwz.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zdv.birdmap.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yac.havefunace.top

JS:   new Date("2024-01-02")
来源：http://ytf.yangfankeji.com

TS:   new Date("2024-01-02")
来源：http://xjj.yuanzhike.top

Java: LocalDate.parse("2024-01-02")
来源：http://rso.tanke756.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sor.hammf.cn

Ruby: Date.parse("2024-01-02")
来源：http://nmo.guowangkeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wxa.shuidangran.top

[J04] 时间戳与日期互转
来源：http://rgw.ctjpmb.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jzc.yonumen.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mam.jinyuanbaomall.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tfs.feifeiyinyue.top

TS:   Math.floor(Date.now() / 1000)
来源：http://edk.cashguo.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kfg.hongshengwenyu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jsp.ivvv.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wbn.tian-w.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pfr.yongpay.top

[J05] 时间加减（加 7 天）
来源：http://mkc.hnqzz.top

Py:   now + timedelta(days=7)
来源：http://rft.jinghuilouyu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dft.zhaomingkeji.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hqt.meibo888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bmb.jqgfzy.top

Java: LocalDate.now().plusDays(7)
来源：http://uko.wangshuangyany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://adc.yj202588.top

Ruby: Time.now + 7 * 86400
来源：http://yhv.0kj1m.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hnt.cashguo.top

[J06] 计算两时间之差
来源：http://vdc.zhengqikj.top

Py:   (end - start).total_seconds()
来源：http://unc.jqgfzy.top

PHP:  $end->diff($start)->days;
来源：http://gzd.mhx1999.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dni.yongpay.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ppu.shanyushiyangkeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://ocs.ctjpmb.com

Go:   end.Sub(start).Hours()
来源：http://sev.wangdashe.top

Ruby: end - start                 # 返回秒数
来源：http://llk.jqgfzy.top

C#:   (end - start).TotalSeconds
来源：http://uys.nanxinkj.top

[J07] 比较两个日期
来源：http://xbz.sjlbkw.cn

Py:   d1 < d2;  d1 == d2
来源：http://ahk.aizwys.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ulk.hnqzz.top

JS:   d1.getTime() < d2.getTime()
来源：http://dyy.shanyushiyangtech.top

TS:   d1.getTime() < d2.getTime()
来源：http://nep.dianchejie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hku.feifeiyinyue.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fii.nanxinkj.top

Ruby: d1 < d2;  d1 == d2
来源：http://gpf.yj20258888.top

C#:   d1 < d2;  d1 == d2
来源：http://fcq.ctjpmb.com

[J08] 提取年月日与星期
来源：http://vnk.zdqjudy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ksi.ydzc1.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uez.zhixingplan.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://afv.meibo888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xli.quarkkingdee.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://asl.andypj.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mib.redwolf501.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dry.cdnleiting.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gij.cashguo.top

[J09] 时区处理
来源：http://bkq.ivvv.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ezk.zdqjudy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gjq.yueranfly.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dfd.yanxiufei.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wps.jiagoushi.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kdr.chenjidiqi.icu

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pqh.sjlbkw.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qid.uphjek.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mmh.fengsongda.top

[J10] 取今天 / 本月第一天
来源：http://iwo.zhaomingkeji.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://gin.xuetiantiany.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yyx.sysykeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://agr.xuanzx.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yzq.svipenyu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yec.ywan-chungtsiang.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lat.nanxinkj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nqc.52xcode.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fpk.vehdjk.com

================================================================================
来源：http://slo.fktsv.cn

K. JSON 与序列化
来源：http://lzj.jyoumei.cn

================================================================================
来源：http://wvn.9152youxi.cn

[K01] 对象转 JSON 字符串
来源：http://ddm.zhiwuduotai.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xpn.zdbjq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hct.hongshengwenyu.top

JS:   JSON.stringify(obj)
来源：http://mvh.hammf.cn

TS:   JSON.stringify(obj)
来源：http://rjw.chenlongwang.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xpz.jlsjyb.cn

Go:   json.Marshal(obj)
来源：http://xww.zhengqikj.top

Ruby: obj.to_json                                     // require "json"
来源：http://kqv.fehbvm.com

C#:   JsonSerializer.Serialize(obj)
来源：http://xzk.pengpengdd.cyou

[K02] JSON 字符串转对象
来源：http://yga.jianghu66.top

Py:   json.loads(s)
来源：http://gyq.aibaodan.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://slr.guannengcc.top

JS:   JSON.parse(s)
来源：http://kon.jqgfzy.top

TS:   JSON.parse(s)
来源：http://gbl.redwolf501.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cmn.shangyingyoupin.top

Go:   json.Unmarshal(data, &v)
来源：http://ovb.cashguo.top

Ruby: JSON.parse(s)
来源：http://cvu.gogol.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rrt.cashguo.top

[K03] JSON 美化输出（带缩进）
来源：http://dfg.yj20258888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hxq.cheryme.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kun.yanxiufei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lov.andypj.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://bzl.hcnkem.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hyo.yueranfly.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pha.jinqigufen.top

Ruby: JSON.pretty_generate(obj)
来源：http://dgo.hnqzz.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fzu.daria6918.cn

[K04] 读取 JSON 文件
来源：http://qdo.yj20258.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ubn.daria6918.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ixj.pycfn.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://txj.meibo888.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cau.wangshuangyany.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sxt.tanke756.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vvo.hongshengwenyu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://zwy.zhixingplan.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://quw.dianchejie.cn

[K05] 深拷贝对象
来源：http://kzq.xylfe.cn

Py:   copy.deepcopy(obj)
来源：http://sww.sysykeji.top

PHP:  unserialize(serialize($obj));
来源：http://pgi.feifeiyinyue.top

JS:   structuredClone(obj)
来源：http://vsg.cashguo.top

TS:   structuredClone(obj)
来源：http://ekd.fengsongda.top

Java: // 手写拷贝构造，或序列化往返
来源：http://xgc.hcnkem.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yxd.bjfxy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kek.fktsv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ecp.bjfxy.top

[K06] 解析 URL 查询串
来源：http://udy.zhoulong.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://apm.snrcjt.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bqv.zhengqikj.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://izo.havefunace.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zmz.cdnleiting.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zms.yfazqb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://pvh.316326.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wnc.ywan-chungtsiang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://izn.pycfn.com

[K07] 进制转换
来源：http://zwd.cdnleiting.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kda.feifeiyinyue.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gfl.zhoulong.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cmc.fktsv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pnf.jlsjyb.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://szb.yonumen.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cbg.gaohongyu789.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tbg.tarul.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://utd.yj20258.top

[K08] 二进制序列化（非 JSON）
来源：http://oav.sweek.top

Py:   pickle.dumps(obj)
来源：http://twd.cucudq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://box.svipenyu.cn

JS:   v8.serialize(obj)        // Node
来源：http://hxv.jinghuilouyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://scw.hnxiangtu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://eja.cashguo.top

Go:   encoding/gob
来源：http://cuu.316326.xyz

Ruby: Marshal.dump(obj)
来源：http://kgp.52xcode.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://syc.9152youxi.cn

================================================================================
来源：http://okh.yj202588.top

L. 网络请求
来源：http://jvp.fanxiaobao.xyz

================================================================================
来源：http://cem.cdnleiting.top

[L01] 发送 GET 请求
来源：http://wci.sweek.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vkw.yongpay.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ewx.gotoacloud.top

JS:   await fetch(url)
来源：http://yps.zhijiandao.cn

TS:   await fetch(url)
来源：http://czr.zhaomingkeji.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gyj.zhaomingkeji.xyz

Go:   resp, err := http.Get(url)
来源：http://saa.pengpengdd.cyou

Ruby: Net::HTTP.get(URI(url))
来源：http://vbc.hywenlv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://apy.dianchejie.cn

[L02] 发送 POST JSON
来源：http://url.cashguo.top

Py:   requests.post(url, json={"a": 1})
来源：http://jvg.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://stx.mhx1999.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ztq.nwbrower.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gad.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ekj.jlsjyb.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vld.xuanzx.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://eww.ctjpmb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cmj.ppjwa.cn

[L03] 设置自定义请求头
来源：http://fyn.jinqigfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://skr.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ynn.zhongyouzk.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oym.andypj.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sle.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cza.gaohongyu789.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sub.cashguo.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lyo.zhongyouzk.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mik.nanxinkj.top

[L04] 设置超时
来源：http://jlq.shzxlz.cn

Py:   requests.get(url, timeout=5)
来源：http://oxo.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rqj.gotoacloud.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lwj.dashuyun.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://onv.sysykeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vkt.fzhhl.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xml.chenzaomai.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ifp.shuidangran.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ypg.52xcode.cn

[L05] 上传文件（multipart）
来源：http://ufs.haohaochexian.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://whu.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wzl.ivvv.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yhs.nanxinkj.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rfp.daria6918.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bse.fehbvm.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jxd.cashguo.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jjj.bbcook.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nha.tarul.cn

[L06] 解析响应为 JSON
来源：http://zid.vqdsnc.cn

Py:   resp.json()
来源：http://pvu.bjfxy.top

PHP:  json_decode($body, true);
来源：http://icl.ctjpmb.com

JS:   await resp.json()
来源：http://gwm.cheryme.top

TS:   await resp.json()
来源：http://tdu.smart0.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gnf.hesvh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qam.hongshengwenyu.top

Ruby: JSON.parse(resp.body)
来源：http://vcz.yueranfly.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jaz.bjfxy.top

[L07] 处理 HTTP 状态码
来源：http://mpv.vehdjk.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://loe.hfpthk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vzr.chenzaomai.com

JS:   resp.ok;  resp.status
来源：http://hlv.jqgfzy.top

TS:   resp.ok;  resp.status
来源：http://jac.yvedp.cn

Java: resp.statusCode()
来源：http://tnr.yanxiufei.cn

Go:   resp.StatusCode
来源：http://jmx.9152youxi.cn

Ruby: resp.code.to_i
来源：http://vqy.ywan-chungtsiang.top

C#:   (int)resp.StatusCode
来源：http://zma.jinqigfzy.top

[L08] 并发请求多个地址
来源：http://mhr.sysykeji.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ytj.hesvh.cn

PHP:  curl_multi_init() 系列
来源：http://ezp.hesvh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fje.fzhhl.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lsn.sxryk.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://obl.jqgufenzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xif.zhengqikj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kqu.quarkkingdee.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cqg.hfpthk.cn

================================================================================
来源：http://bsz.yongpay.top

M. 命令行 / 进程 / 环境
来源：http://jfb.shanyushiyangkeji.top


<!-- 参考信息 -->