代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mnk.jlsjyb.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://npu.cqqwz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bku.chenzaomai.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vom.tian-w.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hko.hesvh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jri.fengsongda.top

[I04] 正则替换
来源：http://uzz.ydjk.org.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hgq.iojbl.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nho.yj20258.top

JS:   s.replace(/\d+/g, "#")
来源：http://lwn.dashuyun.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bmn.c1oappe.top

Java: s.replaceAll("\\d+", "#")
来源：http://whh.vehdjk.com

Go:   re.ReplaceAllString(s, "#")
来源：http://nwj.gaohongyu789.top

Ruby: s.gsub(/\d+/, "#")
来源：http://fge.nanxinkj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://djl.bbcook.cn

[I05] 按正则拆分
来源：http://peu.zhoulong.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://pex.yanxiufei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tfp.zhoulong.xyz

JS:   s.split(/\s*,\s*/)
来源：http://ibr.gzhubu.top

TS:   s.split(/\s*,\s*/)
来源：http://hot.yangfankeji.com

Java: s.split("\\s*,\\s*")
来源：http://flq.ydjk.org.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zpc.havefunace.top

Ruby: s.split(/\s*,\s*/)
来源：http://qjj.sweek.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fls.tanke756.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ira.feifeiyinyue.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ugw.uphjek.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dcw.chenzaomai.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ewg.vqdsnc.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jut.mhx1999.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ama.hfpthk.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kbc.ivvv.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ldc.zhiwuduotai.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ccg.tarul.cn

[I07] 忽略大小写与多行模式
来源：http://qxu.feifeiyinyue.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hos.fanxiaobao.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vks.ydzc1.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uvh.daria6918.cn

TS:   /error/gim
来源：http://juk.c1oappe.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vps.cqqwz.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rcv.jlsjyb.cn

Ruby: s.scan(/error/i)
来源：http://krh.hnxiangtu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xbh.andypj.xyz

[I08] 贪婪与非贪婪匹配
来源：http://zij.wangshuangyany.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hmd.sweek.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://atp.0kj1m.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fvj.yanxiufei.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://foh.9152youxi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://edi.sufxvd.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://plx.iojbl.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tuh.ydzc1.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sta.xuanzx.com

================================================================================
来源：http://gbz.nwbrower.top

J. 日期与时间
来源：http://wah.jqgufenzy.top

================================================================================
来源：http://hbp.yonumen.top

[J01] 获取当前时间
来源：http://ecl.vqdsnc.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://oxp.zycfv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ygs.vqdsnc.cn

JS:   new Date();  Date.now()
来源：http://zua.jyoumei.cn

TS:   new Date();  Date.now()
来源：http://inn.yanxiufei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nce.316326.xyz

Go:   time.Now()
来源：http://chk.nanxuanxn.top

Ruby: Time.now
来源：http://nht.fehbvm.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://avp.yvedp.cn

[J02] 格式化输出
来源：http://qqj.quarkkingdee.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dxs.hywenlv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cki.shangyingyoupin.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pyi.zycfv.cn

TS:   d.toISOString()
来源：http://uos.hnqzz.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ywc.gzhubu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vwg.shanyushiyangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://agd.tarul.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://odi.fengsongda.top

[J03] 字符串解析为日期
来源：http://zbr.guannengcc.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ozv.aibaodan.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://isf.hesvh.cn

JS:   new Date("2024-01-02")
来源：http://rgw.ydzc1.top

TS:   new Date("2024-01-02")
来源：http://cgg.chenlongwang.top

Java: LocalDate.parse("2024-01-02")
来源：http://apk.zhijiandao.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vex.shuidangran.top

Ruby: Date.parse("2024-01-02")
来源：http://jfw.hywenlv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://haj.cheryme.top

[J04] 时间戳与日期互转
来源：http://fvw.yongpay.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fah.shangyingyoupin.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fkd.bbcook.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ieb.yanxiufei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://srb.yvedp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oje.chenjidiqi.icu

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cer.jianghu66.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jmv.zhijiandao.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kde.fanxiaobao.xyz

[J05] 时间加减（加 7 天）
来源：http://mpc.dianchejie.cn

Py:   now + timedelta(days=7)
来源：http://jzs.ywan-chungtsiang.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://szu.hnxiangtu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nja.chenjidiqi.icu

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zda.sjlbkw.cn

Java: LocalDate.now().plusDays(7)
来源：http://wqj.c1oappe.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jsv.yuanzhike.top

Ruby: Time.now + 7 * 86400
来源：http://ufd.gzhubu.top

C#:   DateTime.Now.AddDays(7)
来源：http://pom.zhiwuduotai.top

[J06] 计算两时间之差
来源：http://lvv.xylfe.cn

Py:   (end - start).total_seconds()
来源：http://may.dianchejie.cn

PHP:  $end->diff($start)->days;
来源：http://svj.fzhhl.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://akb.hnqzz.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zpm.yuanzhike.top

Java: Duration.between(start, end).toSeconds()
来源：http://cpf.nanxuanxn.top

Go:   end.Sub(start).Hours()
来源：http://crf.wangshuangyany.cn

Ruby: end - start                 # 返回秒数
来源：http://jpw.smart0.xyz

C#:   (end - start).TotalSeconds
来源：http://udp.xinyue.icu

[J07] 比较两个日期
来源：http://tpa.hfpthk.cn

Py:   d1 < d2;  d1 == d2
来源：http://ngl.bbcook.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://occ.daria6918.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gvo.zhengqikj.top

TS:   d1.getTime() < d2.getTime()
来源：http://jqi.gogol.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ubb.fzhhl.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ahk.sufxvd.cn

Ruby: d1 < d2;  d1 == d2
来源：http://phg.jiagoushi.top

C#:   d1 < d2;  d1 == d2
来源：http://glw.hesvh.cn

[J08] 提取年月日与星期
来源：http://pek.zhixingplan.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xce.ydzc1.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mey.nanxinkj.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dpk.xylfe.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xju.pycfn.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qqi.jianghu66.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jey.redwolf501.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://apr.yongpay.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kqn.ydzc1.top

[J09] 时区处理
来源：http://yhv.dashuyun.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dhm.jlsjyb.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xtu.chenzaomai.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yct.zhixingplan.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dpo.haohaochexian.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uoc.cqqwz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qzq.wangdashe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://oyx.jyoumei.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://aeh.9152youxi.cn

[J10] 取今天 / 本月第一天
来源：http://mfs.fengsongda.top

Py:   date.today();  date.today().replace(day=1)
来源：http://eiy.zhongyouzk.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yxm.fengsongda.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://smw.hywenlv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rmr.fehbvm.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sgt.jinghuilouyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qet.yj20258888.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wfo.yj20258.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hhs.cdnleiting.top

================================================================================
来源：http://qmf.zycfv.cn

K. JSON 与序列化
来源：http://xir.haohaochexian.top

================================================================================
来源：http://tzk.pycfn.com

[K01] 对象转 JSON 字符串
来源：http://mkq.chenjidiqi.icu

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://aei.xuetiantiany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kyt.ppjwa.cn

JS:   JSON.stringify(obj)
来源：http://nty.fanxiaobao.xyz

TS:   JSON.stringify(obj)
来源：http://yoc.gogol.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lsr.zhongyouzk.top

Go:   json.Marshal(obj)
来源：http://wrh.tarul.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kzg.cqqwz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dux.shuidangran.top

[K02] JSON 字符串转对象
来源：http://lxj.zhongyouzk.top

Py:   json.loads(s)
来源：http://vot.dianchejie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ixg.sjlbkw.cn

JS:   JSON.parse(s)
来源：http://jct.jlsjyb.cn

TS:   JSON.parse(s)
来源：http://zrk.cucudq.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kgn.xziqi.cn

Go:   json.Unmarshal(data, &v)
来源：http://yxo.jyoumei.cn

Ruby: JSON.parse(s)
来源：http://knu.kuanghao11.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://drg.redwolf501.top

[K03] JSON 美化输出（带缩进）
来源：http://wee.kuanghao11.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zsz.yueranfly.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rjh.cheryme.top

JS:   JSON.stringify(obj, null, 2)
来源：http://gnn.0kj1m.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://bkj.zhengqikj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kim.jinyuanbaomall.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pbt.sysykeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://wyt.pengpengdd.cyou

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pxr.ivvv.top

[K04] 读取 JSON 文件
来源：http://rny.yongpay.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jkb.cashguo.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://euy.birdmap.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://afl.xuetiantiany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lai.xingfuxueyuan.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fvz.jiagoushi.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kqp.snrcjt.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dth.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zmk.xziqi.cn

[K05] 深拷贝对象
来源：http://aza.ivvv.top

Py:   copy.deepcopy(obj)
来源：http://mtq.pengpengdd.cyou

PHP:  unserialize(serialize($obj));
来源：http://gbz.zhixingplan.top

JS:   structuredClone(obj)
来源：http://aww.hesvh.cn

TS:   structuredClone(obj)
来源：http://ieu.xziqi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cjf.jianghu66.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vrj.pengpengdd.cyou

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pzz.xuanzx.com

C#:   // 序列化往返，或自定义 Clone
来源：http://xvp.cheryme.top

[K06] 解析 URL 查询串
来源：http://ron.jqgfzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rer.shangyingyoupin.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mwu.tian-w.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mlf.jlsjyb.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lib.nanxinkj.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mxe.yonumen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://wow.zhengqikj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qjd.xziqi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cdk.chenzaomai.com

[K07] 进制转换
来源：http://qws.hesvh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://myw.jiagoushi.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://plc.cqqwz.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fwd.hcnkem.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sur.yueranfly.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qhi.uphjek.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vje.yanxiufei.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fsb.zhaomingkeji.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lcx.vehdjk.com

[K08] 二进制序列化（非 JSON）
来源：http://jff.hfpthk.cn

Py:   pickle.dumps(obj)
来源：http://inn.zdqjudy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xxe.xinyue.icu

JS:   v8.serialize(obj)        // Node
来源：http://ubv.guannengcc.top

TS:   v8.serialize(obj)        // Node
来源：http://tky.ybcxt.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pfm.snrcjt.cn

Go:   encoding/gob
来源：http://jvp.jinqigufen.top

Ruby: Marshal.dump(obj)
来源：http://ryh.jiagoushi.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pzb.uphjek.com

================================================================================
来源：http://fcc.shangyingyoupin.top

L. 网络请求
来源：http://zxk.zdbjq.cn

================================================================================
来源：http://pxd.zdbjq.cn

[L01] 发送 GET 请求
来源：http://uxl.tian-w.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dzd.zycfv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uin.aibaodan.cn

JS:   await fetch(url)
来源：http://hdf.gotoacloud.top

TS:   await fetch(url)
来源：http://dxa.daria6918.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fep.xingfuxueyuan.xyz

Go:   resp, err := http.Get(url)
来源：http://mhu.cdnleiting.top

Ruby: Net::HTTP.get(URI(url))
来源：http://gal.yongpay.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://imh.ywan-chungtsiang.top

[L02] 发送 POST JSON
来源：http://gsl.yanxiufei.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hfr.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tvv.haohaochexian.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hwd.nanxinkj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uek.bjfxy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hzq.kuanghao11.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://del.fanxiaobao.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jte.meibo888.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cvi.c1oappe.top

[L03] 设置自定义请求头
来源：http://rgx.cucudq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uyw.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hqu.sweek.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rkq.gotoacloud.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uny.pycfn.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ftv.bjfxy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dmr.jianghu66.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xfu.cucudq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fyu.sufxvd.cn

[L04] 设置超时
来源：http://lpg.9152youxi.cn

Py:   requests.get(url, timeout=5)
来源：http://qzb.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://btm.shanyushiyangtech.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cdn.hysaishi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mzu.zhijiandao.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bmw.pycfn.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ham.0kj1m.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kaz.xingfuxueyuan.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://enz.andypj.xyz

[L05] 上传文件（multipart）
来源：http://qne.zhixingplan.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wfg.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bgl.hfpthk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gvb.fengsongda.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eci.dashuyun.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pqh.chenlongwang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uve.daxiang520.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://plk.xuetiantiany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zyv.uphjek.com

[L06] 解析响应为 JSON
来源：http://aox.52xcode.cn

Py:   resp.json()
来源：http://ret.uphjek.com

PHP:  json_decode($body, true);
来源：http://acj.yj202588.top

JS:   await resp.json()
来源：http://kdt.tian-w.cn

TS:   await resp.json()
来源：http://gow.nwbrower.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dyi.yueranfly.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ltt.ydzc1.top

Ruby: JSON.parse(resp.body)
来源：http://gsr.snrcjt.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://frk.zhixingplan.top

[L07] 处理 HTTP 状态码
来源：http://wez.316326.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pls.zhiwuduotai.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bkm.chenjidiqi.icu

JS:   resp.ok;  resp.status
来源：http://iud.ivvv.top

TS:   resp.ok;  resp.status
来源：http://mpi.nanxuanxn.top

Java: resp.statusCode()
来源：http://qfp.dianchejie.cn

Go:   resp.StatusCode
来源：http://dhu.vqdsnc.cn

Ruby: resp.code.to_i
来源：http://mju.tarul.cn

C#:   (int)resp.StatusCode
来源：http://yig.sysykeji.top

[L08] 并发请求多个地址
来源：http://pgc.guowangkeji.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xik.nanxinkj.top

PHP:  curl_multi_init() 系列
来源：http://klt.jiagoushi.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tci.yueranfly.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zjv.nanxinkj.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sph.daria6918.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://plj.uphjek.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fca.zhongyouzk.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qti.pengpengdd.cyou

================================================================================
来源：http://zbq.yueranfly.top

M. 命令行 / 进程 / 环境
来源：http://swa.hfpthk.cn

================================================================================
来源：http://rup.tian-w.cn

[M01] 读取命令行参数
来源：http://vhk.cdnleiting.top

Py:   sys.argv[1:]
来源：http://wfa.ybcxt.top

PHP:  $argv;  $argc;
来源：http://url.fanxiaobao.xyz


<!-- 参考信息 -->