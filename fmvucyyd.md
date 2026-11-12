代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://ndc.jiagoushi.top

JS:   toString() { return this.name; }
来源：http://sxk.gogol.net.cn

TS:   toString(): string { return this.name; }
来源：http://rmd.jqgufenzy.top

Java: @Override public String toString() { return name; }
来源：http://yxk.redwolf501.top

Go:   func (u User) String() string { return u.Name }
来源：http://rtk.nanxinkj.top

Ruby: def to_s; @name; end
来源：http://hmf.gaohongyu789.top

C#:   public override string ToString() => Name;
来源：http://aqn.jianghu66.top

[G13] 判断对象类型
来源：http://gxg.havefunace.top

Py:   isinstance(u, User)
来源：http://xji.yuxming.cn

PHP:  $u instanceof User
来源：http://oez.sweek.top

JS:   u instanceof User
来源：http://lma.gaohongyu789.top

TS:   u instanceof User
来源：http://jua.cashguo.top

Java: u instanceof User
来源：http://imm.jqgfzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://bho.316326.xyz

Ruby: u.is_a?(User)
来源：http://bhp.guowangkeji.top

C#:   u is User
来源：http://fvn.ywan-chungtsiang.top

[G14] 数据类 / record
来源：http://rwm.feifeiyinyue.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lzt.sufxvd.cn

PHP:  // 用 readonly 属性模拟
来源：http://xam.zhiwuduotai.top

JS:   // 无内置：普通类或对象字面量
来源：http://ghd.ydzc1.top

TS:   type User = { name: string; age: number };
来源：http://fhz.hnqzz.top

Java: record User(String name, int age) {}
来源：http://lfu.wangshuangyany.cn

Go:   type User struct { Name string; Age int }
来源：http://aah.yvedp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hqj.jinqigufen.top

C#:   record User(string Name, int Age);
来源：http://ner.chenlongwang.top

[G15] 枚举
来源：http://qif.havefunace.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oxf.cashguo.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://icd.xziqi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iro.316326.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sgd.yfazqb.com

Java: enum Color { RED, GREEN }
来源：http://wig.0kj1m.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pqo.tarul.cn

Ruby: Color = %i[red green].freeze
来源：http://mun.vqdsnc.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cff.shanyushiyangkeji.top

[G16] 对象转数组 / 字典
来源：http://igu.jqgufenzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://anu.nanxuanxn.top

PHP:  get_object_vars($obj);
来源：http://jdv.vehdjk.com

JS:   Object.entries(obj)
来源：http://wxr.aibaodan.cn

TS:   Object.entries(obj)
来源：http://kjv.ydjk.org.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rus.zhixingplan.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://pjq.uphjek.com

Ruby: obj.instance_variables
来源：http://tfd.hfpthk.cn

C#:   // 用反射或 System.Text.Json
来源：http://pvv.zhongyouzk.top

================================================================================
来源：http://aai.yfazqb.com

H. 异常与错误处理
来源：http://asd.fengsongda.top

================================================================================
来源：http://nja.shanyushiyangkeji.top

[H01] try / catch 基础
来源：http://qes.guannengcc.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xoi.zhongyouzk.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://osq.zdbjq.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tce.daxiang520.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://eix.shanyushiyangtech.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ftg.cashguo.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://svu.52xcode.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kmp.havefunace.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://thg.sysykeji.top

[H02] finally / ensure 收尾
来源：http://xkx.tanke756.top

Py:   try: f()⏎finally: cleanup()
来源：http://xvo.zdqjudy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://myo.316326.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://epf.shanyushiyangtech.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mcj.sufxvd.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uzi.nwbrower.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://vil.yuanzhike.top

Ruby: begin; f; ensure; cleanup; end
来源：http://aap.ybcxt.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://vgz.iojbl.cn

[H03] 主动抛出异常
来源：http://nab.snrcjt.cn

Py:   raise ValueError("错误信息")
来源：http://ere.shangyingyoupin.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ntv.yonumen.top

JS:   throw new Error("错误信息");
来源：http://bkl.cdnleiting.top

TS:   throw new Error("错误信息");
来源：http://mkp.yj202588.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ozn.vehdjk.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://isd.aibaodan.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fsr.hongshengwenyu.top

C#:   throw new ArgumentException("错误信息");
来源：http://gbm.jinghuilouyu.cn

[H04] 自定义异常类型
来源：http://xwm.wangshuangyany.cn

Py:   class MyError(Exception): pass
来源：http://nwa.c1oappe.top

PHP:  class MyError extends RuntimeException {}
来源：http://jml.vehdjk.com

JS:   class MyError extends Error {}
来源：http://inx.yj202588.top

TS:   class MyError extends Error {}
来源：http://ixt.hesvh.cn

Java: class MyException extends RuntimeException {}
来源：http://mhu.gaohongyu789.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vwg.xuetiantiany.cn

Ruby: class MyError < StandardError; end
来源：http://bma.uphjek.com

C#:   class MyException : Exception {}
来源：http://ufe.tarul.cn

[H05] 捕获特定类型
来源：http://typ.daxiang520.top

Py:   except ValueError as e:
来源：http://ihu.yuanzhike.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lsl.xylfe.cn

JS:   if (e instanceof TypeError) {}
来源：http://kft.xuanzx.com

TS:   if (e instanceof TypeError) {}
来源：http://iax.fehbvm.com

Java: catch (IOException | SQLException e) {}
来源：http://fey.fehbvm.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pme.redwolf501.top

Ruby: rescue ArgumentError => e
来源：http://fkv.bjfxy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kzo.jinyuanbaomall.cn

[H06] 可选值 / 空值安全访问
来源：http://hnh.yonumen.top

Py:   value = d.get("k") or default
来源：http://sfn.zhaomingkeji.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://icf.wangdashe.top

JS:   obj?.a?.b;  d ?? default
来源：http://kvn.ybcxt.top

TS:   obj?.a?.b;  d ?? default
来源：http://yiz.zhaomingkeji.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://grx.0kj1m.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ifn.zhijiandao.cn

Ruby: d&.dig(:a, :b)
来源：http://xdp.mhx1999.top

C#:   obj?.A?.B ?? default
来源：http://nxk.chenjidiqi.icu

[H07] 断言
来源：http://lin.zhijiandao.cn

Py:   assert x > 0, "必须为正"
来源：http://aoc.smart0.xyz

PHP:  assert($x > 0);
来源：http://jbh.kuanghao11.cn

JS:   console.assert(x > 0);
来源：http://ajw.jinghuilouyu.cn

TS:   console.assert(x > 0);
来源：http://cbp.daria6918.cn

Java: assert x > 0 : "必须为正";
来源：http://yhd.jlsjyb.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://grh.nanxinkj.top

Ruby: raise "必须为正" unless x > 0
来源：http://gtd.feifeiyinyue.top

C#:   Debug.Assert(x > 0);
来源：http://quv.smart0.xyz

[H08] 获取错误信息与堆栈
来源：http://pri.feifeiyinyue.top

Py:   str(e);  traceback.format_exc()
来源：http://fig.cheryme.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fsb.ctjpmb.com

JS:   e.message;  e.stack
来源：http://vie.cheryme.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://buy.haohaochexian.top

Java: e.getMessage();  e.printStackTrace()
来源：http://rnj.tanke756.top

Go:   err.Error()
来源：http://uvr.ctjpmb.com

Ruby: e.message;  e.backtrace
来源：http://ady.zycfv.cn

C#:   e.Message;  e.StackTrace
来源：http://lxn.shanyushiyangtech.top

[H09] 带错误码的异常
来源：http://yzl.nanxinkj.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bqs.nanxinkj.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qng.hfpthk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pax.gotoacloud.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fgb.cdnleiting.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://miw.yvedp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mwc.yvedp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fku.yfazqb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://bgs.svipenyu.cn

[H10] 资源自动释放
来源：http://tol.hnqzz.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://rus.fanxiaobao.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ytk.gzhubu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mxx.xylfe.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zil.yonumen.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jjh.ehwqpu.com

Go:   defer f.Close()
来源：http://snr.cdnleiting.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uas.birdmap.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jxu.yonumen.top

================================================================================
来源：http://mwb.smart0.xyz

I. 正则表达式
来源：http://xwo.hywenlv.cn

================================================================================
来源：http://iyo.smart0.xyz

[I01] 判断是否匹配
来源：http://jsc.pycfn.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kbt.nwbrower.top

PHP:  preg_match('/\d+/', $s);
来源：http://gdp.xuetiantiany.cn

JS:   /\d+/.test(s)
来源：http://nbs.birdmap.top

TS:   /\d+/.test(s)
来源：http://ujd.iojbl.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tao.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fgb.cheryme.top

Ruby: s.match?(/\d+/)
来源：http://ulz.yonumen.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nsl.cheryme.top

[I02] 提取所有匹配
来源：http://eia.xziqi.cn

Py:   re.findall(r"\d+", s)
来源：http://nmt.epnwcf.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ecj.jiagoushi.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qsx.zhongyouzk.top

TS:   s.match(/\d+/g)
来源：http://wmd.ehwqpu.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ank.cucudq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pml.quarkkingdee.top

Ruby: s.scan(/\d+/)
来源：http://gmv.gotoacloud.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fef.vehdjk.com

[I03] 提取捕获分组
来源：http://ogz.ybcxt.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://duz.smart0.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hzc.yueranfly.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jkp.gogol.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wkp.tarul.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nhf.jinqigfzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fvt.vehdjk.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ots.hammf.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://biv.316326.xyz

[I04] 正则替换
来源：http://qcz.andypj.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://ire.ehwqpu.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fwc.xylfe.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wxj.jinqigufen.top

TS:   s.replace(/\d+/g, "#")
来源：http://cqs.yonumen.top

Java: s.replaceAll("\\d+", "#")
来源：http://djx.jyoumei.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bro.yangfankeji.com

Ruby: s.gsub(/\d+/, "#")
来源：http://vmu.jyoumei.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dkp.andypj.xyz

[I05] 按正则拆分
来源：http://cmf.sxryk.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://okq.jinqigufen.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fpm.jqgfzy.top

JS:   s.split(/\s*,\s*/)
来源：http://vwb.hnqzz.top

TS:   s.split(/\s*,\s*/)
来源：http://ing.zhengqikj.top

Java: s.split("\\s*,\\s*")
来源：http://ywb.jqgufenzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jwx.c1oappe.top

Ruby: s.split(/\s*,\s*/)
来源：http://vpz.bjfxy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bml.cucudq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zsw.svipenyu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jxw.hywenlv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jfl.uphjek.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sdw.cheryme.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wuf.ctjpmb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pei.hnxiangtu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jac.fzhhl.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qvy.jinqigfzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oww.hnxiangtu.top

[I07] 忽略大小写与多行模式
来源：http://zqh.snrcjt.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xun.meibo888.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hcb.svipenyu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wdm.hcnkem.com

TS:   /error/gim
来源：http://krf.aizwys.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wqh.yfazqb.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qod.hongshengwenyu.top

Ruby: s.scan(/error/i)
来源：http://mij.havefunace.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qzs.shuidangran.top

[I08] 贪婪与非贪婪匹配
来源：http://tcs.zhengqikj.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://izo.jinyuanbaomall.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vih.jlsjyb.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ngd.quarkkingdee.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://afm.feifeiyinyue.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ubw.daxiang520.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xfr.kuanghao11.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vsb.zhixingplan.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xmh.tian-w.cn

================================================================================
来源：http://bwe.svipenyu.cn

J. 日期与时间
来源：http://ghx.sysykeji.top

================================================================================
来源：http://tje.yuxming.cn

[J01] 获取当前时间
来源：http://wgl.wangdashe.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://yqn.smart0.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tkf.xingfuxueyuan.xyz

JS:   new Date();  Date.now()
来源：http://yju.yueranfly.top

TS:   new Date();  Date.now()
来源：http://bwf.ywan-chungtsiang.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ktg.aibaodan.cn

Go:   time.Now()
来源：http://tlz.yj202588.top

Ruby: Time.now
来源：http://ihj.tanke756.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blp.aizwys.cn

[J02] 格式化输出
来源：http://eee.sufxvd.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wqf.xuetiantiany.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hqv.tian-w.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xzk.pengpengdd.cyou

TS:   d.toISOString()
来源：http://mbi.316326.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jft.jiagoushi.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zip.xziqi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fpw.fanxiaobao.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kss.wangshuangyany.cn

[J03] 字符串解析为日期
来源：http://dew.pycfn.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vya.yangfankeji.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gfy.yangfankeji.com

JS:   new Date("2024-01-02")
来源：http://vjg.tianlin.xyz

TS:   new Date("2024-01-02")
来源：http://kst.chenzaomai.com

Java: LocalDate.parse("2024-01-02")
来源：http://ymr.shanyushiyangtech.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eyq.guannengcc.top

Ruby: Date.parse("2024-01-02")
来源：http://yfn.gogol.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yyq.fengsongda.top

[J04] 时间戳与日期互转
来源：http://lkn.guowangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dxk.zhoulong.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jae.daria6918.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yeg.ehwqpu.com

TS:   Math.floor(Date.now() / 1000)
来源：http://qgt.hywenlv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pdf.yfazqb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nft.yueranfly.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://syp.316326.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qpk.birdmap.top

[J05] 时间加减（加 7 天）
来源：http://reu.shuidangran.top

Py:   now + timedelta(days=7)
来源：http://zsh.zhoulong.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://wbd.fehbvm.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mij.uphjek.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kuj.mhx1999.top

Java: LocalDate.now().plusDays(7)
来源：http://oyc.hnqzz.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xsy.hammf.cn

Ruby: Time.now + 7 * 86400
来源：http://djz.yuxming.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jqv.wangdashe.top

[J06] 计算两时间之差
来源：http://joq.tianlin.xyz

Py:   (end - start).total_seconds()
来源：http://lmn.feifeiyinyue.top

PHP:  $end->diff($start)->days;
来源：http://bwz.hesvh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fmy.cheryme.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lsy.ivvv.top

Java: Duration.between(start, end).toSeconds()
来源：http://rcv.yanxiufei.cn

Go:   end.Sub(start).Hours()
来源：http://pna.xylfe.cn

Ruby: end - start                 # 返回秒数
来源：http://kez.shangyingyoupin.top

C#:   (end - start).TotalSeconds
来源：http://jjw.hnqzz.top

[J07] 比较两个日期
来源：http://oma.bjfxy.top

Py:   d1 < d2;  d1 == d2
来源：http://pwx.gotoacloud.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xgy.yuanzhike.top

JS:   d1.getTime() < d2.getTime()
来源：http://bzy.meibo888.top

TS:   d1.getTime() < d2.getTime()
来源：http://qdy.ctjpmb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sde.ydzc1.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://orp.vehdjk.com

Ruby: d1 < d2;  d1 == d2
来源：http://vye.ppjwa.cn

C#:   d1 < d2;  d1 == d2
来源：http://jws.xingfuxueyuan.xyz

[J08] 提取年月日与星期
来源：http://ckj.smart0.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rii.shanyushiyangkeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bts.jqgfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xev.haohaochexian.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rlm.daxiang520.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jdf.yj202588.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tmp.yj20258888.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://apw.chenjidiqi.icu

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ogd.hongshengwenyu.top

[J09] 时区处理
来源：http://eli.cashguo.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://oeb.iojbl.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://isi.pycfn.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kek.tarul.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cmr.ydzc1.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pez.gogol.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dve.jinqigufen.top

Ruby: Time.now.getlocal("+08:00")
来源：http://cor.chenlongwang.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sgi.sjlbkw.cn

[J10] 取今天 / 本月第一天
来源：http://nwg.gaohongyu789.top

Py:   date.today();  date.today().replace(day=1)
来源：http://lbb.birdmap.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sdx.birdmap.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ubm.aibaodan.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lmm.yvedp.cn


<!-- 参考信息 -->