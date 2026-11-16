代发 wailian999

Ruby: attr_accessor :name
来源：http://adc.fktsv.cn

C#:   public string Name { get; set; }
来源：http://kje.jyoumei.cn

[G12] 对象转字符串
来源：http://tce.yvedp.cn

Py:   def __str__(self): return self.name
来源：http://itn.jinqigufen.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ssl.yvedp.cn

JS:   toString() { return this.name; }
来源：http://lqh.sweek.top

TS:   toString(): string { return this.name; }
来源：http://mwu.zhijiandao.cn

Java: @Override public String toString() { return name; }
来源：http://rdq.hfpthk.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bpk.cheryme.top

Ruby: def to_s; @name; end
来源：http://sqk.shanyushiyangtech.top

C#:   public override string ToString() => Name;
来源：http://xfy.jianghu66.top

[G13] 判断对象类型
来源：http://yxh.shangyingyoupin.top

Py:   isinstance(u, User)
来源：http://osf.yanxiufei.cn

PHP:  $u instanceof User
来源：http://ife.yonumen.top

JS:   u instanceof User
来源：http://xol.xingfuxueyuan.xyz

TS:   u instanceof User
来源：http://hvm.jlsjyb.cn

Java: u instanceof User
来源：http://uyu.bbcook.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gcq.ctjpmb.com

Ruby: u.is_a?(User)
来源：http://vef.hesvh.cn

C#:   u is User
来源：http://vkc.sxryk.cn

[G14] 数据类 / record
来源：http://qvd.smart0.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jrb.nanxinkj.top

PHP:  // 用 readonly 属性模拟
来源：http://cbu.jqgufenzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://syo.fzhhl.top

TS:   type User = { name: string; age: number };
来源：http://kxa.yanxiufei.cn

Java: record User(String name, int age) {}
来源：http://gsg.yj202588.top

Go:   type User struct { Name string; Age int }
来源：http://qnz.fzhhl.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://elq.tianlin.xyz

C#:   record User(string Name, int Age);
来源：http://ixr.ctjpmb.com

[G15] 枚举
来源：http://swy.uphjek.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cxr.xuanzx.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://hgg.xuetiantiany.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://opu.dianchejie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ewp.0kj1m.cn

Java: enum Color { RED, GREEN }
来源：http://uqi.jiagoushi.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ail.9152youxi.cn

Ruby: Color = %i[red green].freeze
来源：http://nvc.daria6918.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nng.nanxuanxn.top

[G16] 对象转数组 / 字典
来源：http://sel.daria6918.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lqw.tian-w.cn

PHP:  get_object_vars($obj);
来源：http://nqc.vqdsnc.cn

JS:   Object.entries(obj)
来源：http://dxb.fzhhl.top

TS:   Object.entries(obj)
来源：http://wyj.quarkkingdee.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vbk.zhixingplan.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://dmx.xuanzx.com

Ruby: obj.instance_variables
来源：http://pyq.hammf.cn

C#:   // 用反射或 System.Text.Json
来源：http://ivs.haohaochexian.top

================================================================================
来源：http://kyn.yj202588.top

H. 异常与错误处理
来源：http://arr.yonumen.top

================================================================================
来源：http://lyg.xuetiantiany.cn

[H01] try / catch 基础
来源：http://igl.yonumen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uuj.52xcode.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://usl.dianchejie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dxb.xuanzx.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jtg.gotoacloud.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tdx.316326.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fop.ivvv.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mbt.shangyingyoupin.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://itw.chenjidiqi.icu

[H02] finally / ensure 收尾
来源：http://edf.daxiang520.top

Py:   try: f()⏎finally: cleanup()
来源：http://ayc.zdqjudy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://nxt.uphjek.com

JS:   try { f(); } finally { cleanup(); }
来源：http://ygh.shanyushiyangtech.top

TS:   try { f(); } finally { cleanup(); }
来源：http://vdm.cucudq.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mlg.uphjek.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://gwr.hfpthk.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mcj.gotoacloud.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://oms.zdbjq.cn

[H03] 主动抛出异常
来源：http://cyj.jqgufenzy.top

Py:   raise ValueError("错误信息")
来源：http://zge.xinyue.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rsc.ydzc1.top

JS:   throw new Error("错误信息");
来源：http://svi.chenzaomai.com

TS:   throw new Error("错误信息");
来源：http://sxz.jinqigfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qba.ehwqpu.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lwt.ehwqpu.com

Ruby: raise ArgumentError, "错误信息"
来源：http://fbf.zdbjq.cn

C#:   throw new ArgumentException("错误信息");
来源：http://toa.birdmap.top

[H04] 自定义异常类型
来源：http://fwc.daxiang520.top

Py:   class MyError(Exception): pass
来源：http://vli.sweek.top

PHP:  class MyError extends RuntimeException {}
来源：http://lbf.jianghu66.top

JS:   class MyError extends Error {}
来源：http://jku.52xcode.cn

TS:   class MyError extends Error {}
来源：http://pok.chenzaomai.com

Java: class MyException extends RuntimeException {}
来源：http://gzl.gotoacloud.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ytf.sxryk.cn

Ruby: class MyError < StandardError; end
来源：http://jud.ppjwa.cn

C#:   class MyException : Exception {}
来源：http://vvs.smart0.xyz

[H05] 捕获特定类型
来源：http://hte.cdnleiting.top

Py:   except ValueError as e:
来源：http://ozz.nanxuanxn.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jeh.tianlin.xyz

JS:   if (e instanceof TypeError) {}
来源：http://utv.xuetiantiany.cn

TS:   if (e instanceof TypeError) {}
来源：http://nta.52xcode.cn

Java: catch (IOException | SQLException e) {}
来源：http://loe.chenzaomai.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yig.cqqwz.cn

Ruby: rescue ArgumentError => e
来源：http://ine.jqgufenzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yxr.bbcook.cn

[H06] 可选值 / 空值安全访问
来源：http://ehk.yj20258.top

Py:   value = d.get("k") or default
来源：http://thx.feifeiyinyue.top

PHP:  $v = $d["k"] ?? null;
来源：http://hyp.ywan-chungtsiang.top

JS:   obj?.a?.b;  d ?? default
来源：http://dmi.mhx1999.top

TS:   obj?.a?.b;  d ?? default
来源：http://ejf.snrcjt.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rav.xuetiantiany.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tzz.fanxiaobao.xyz

Ruby: d&.dig(:a, :b)
来源：http://yzu.nanxuanxn.top

C#:   obj?.A?.B ?? default
来源：http://iku.jianghu66.top

[H07] 断言
来源：http://xwp.shanyushiyangtech.top

Py:   assert x > 0, "必须为正"
来源：http://kan.cqqwz.cn

PHP:  assert($x > 0);
来源：http://dih.uphjek.com

JS:   console.assert(x > 0);
来源：http://whf.yongpay.top

TS:   console.assert(x > 0);
来源：http://bdn.cashguo.top

Java: assert x > 0 : "必须为正";
来源：http://nsv.vqdsnc.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gob.pengpengdd.cyou

Ruby: raise "必须为正" unless x > 0
来源：http://jai.wangshuangyany.cn

C#:   Debug.Assert(x > 0);
来源：http://oob.aibaodan.cn

[H08] 获取错误信息与堆栈
来源：http://yxi.hysaishi.cn

Py:   str(e);  traceback.format_exc()
来源：http://ctu.gotoacloud.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gee.cashguo.top

JS:   e.message;  e.stack
来源：http://vwt.iojbl.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://uqw.c1oappe.top

Java: e.getMessage();  e.printStackTrace()
来源：http://tnc.meibo888.top

Go:   err.Error()
来源：http://xiz.xylfe.cn

Ruby: e.message;  e.backtrace
来源：http://sub.fanxiaobao.xyz

C#:   e.Message;  e.StackTrace
来源：http://mjw.dianchejie.cn

[H09] 带错误码的异常
来源：http://usu.zhengqikj.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://erj.guannengcc.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rfn.shanyushiyangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yaa.jianghu66.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://idy.hnxiangtu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ubq.sufxvd.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://emz.zhixingplan.top

Ruby: raise MyError.new("fail", 500)
来源：http://emf.fehbvm.com

C#:   // 自定义异常类中加 Code 属性
来源：http://orn.pengpengdd.cyou

[H10] 资源自动释放
来源：http://lzc.yfazqb.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://vkp.jyoumei.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sbx.ctjpmb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://acz.daria6918.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sqx.guannengcc.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://idq.hnqzz.top

Go:   defer f.Close()
来源：http://txg.cqqwz.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://coq.bjfxy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tvz.zdbjq.cn

================================================================================
来源：http://myt.yj20258.top

I. 正则表达式
来源：http://zkd.hnxiangtu.top

================================================================================
来源：http://fsn.dianchejie.cn

[I01] 判断是否匹配
来源：http://sub.fanxiaobao.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jjf.kuanghao11.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hrc.jqgufenzy.top

JS:   /\d+/.test(s)
来源：http://zsi.jyoumei.cn

TS:   /\d+/.test(s)
来源：http://wns.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dxh.yj202588.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fbg.jlsjyb.cn

Ruby: s.match?(/\d+/)
来源：http://ctr.xinyue.icu

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sxo.tarul.cn

[I02] 提取所有匹配
来源：http://coe.yj20258.top

Py:   re.findall(r"\d+", s)
来源：http://njy.snrcjt.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://msd.hywenlv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pta.aibaodan.cn

TS:   s.match(/\d+/g)
来源：http://hmw.jinqigufen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hwn.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kwo.guannengcc.top

Ruby: s.scan(/\d+/)
来源：http://kkg.daria6918.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mnx.sjlbkw.cn

[I03] 提取捕获分组
来源：http://wge.9152youxi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kks.uphjek.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://igd.cqqwz.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oyp.yonumen.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bni.fehbvm.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fwi.mhx1999.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dav.mhx1999.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wgt.yuxming.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ftc.snrcjt.cn

[I04] 正则替换
来源：http://svl.dianchejie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qcl.jinqigufen.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ioe.0kj1m.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pzj.dianchejie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qmp.jinqigufen.top

Java: s.replaceAll("\\d+", "#")
来源：http://ufv.yj20258.top

Go:   re.ReplaceAllString(s, "#")
来源：http://rfm.sufxvd.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tic.yueranfly.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cdu.ywan-chungtsiang.top

[I05] 按正则拆分
来源：http://kxa.zhengqikj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ega.bbcook.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wmc.cqqwz.cn

JS:   s.split(/\s*,\s*/)
来源：http://cqx.jianghu66.top

TS:   s.split(/\s*,\s*/)
来源：http://sxp.pengpengdd.cyou

Java: s.split("\\s*,\\s*")
来源：http://nie.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zeq.ehwqpu.com

Ruby: s.split(/\s*,\s*/)
来源：http://gwr.nanxuanxn.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hpv.pycfn.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ytu.jqgufenzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://slo.nanxuanxn.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hey.xziqi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lkc.meibo888.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://icl.zhijiandao.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zcd.yanxiufei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lar.xingfuxueyuan.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://aay.yj20258888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qqz.epnwcf.com

[I07] 忽略大小写与多行模式
来源：http://dca.yuanzhike.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://isp.xuanzx.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yxb.yonumen.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://twj.hnqzz.top

TS:   /error/gim
来源：http://fhw.meibo888.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://anw.cheryme.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jrh.shanyushiyangtech.top

Ruby: s.scan(/error/i)
来源：http://phj.nwbrower.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pnx.chenlongwang.top

[I08] 贪婪与非贪婪匹配
来源：http://otw.uphjek.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cwj.hesvh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ixv.xziqi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hxu.zdbjq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pdu.fengsongda.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xjv.shanyushiyangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mry.dianchejie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tnd.vehdjk.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zrn.shangyingyoupin.top

================================================================================
来源：http://asn.jlsjyb.cn

J. 日期与时间
来源：http://kbo.jianghu66.top

================================================================================
来源：http://vkm.xziqi.cn

[J01] 获取当前时间
来源：http://yhp.svipenyu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://avf.jiagoushi.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bsq.redwolf501.top

JS:   new Date();  Date.now()
来源：http://kfa.hesvh.cn

TS:   new Date();  Date.now()
来源：http://ait.xziqi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yzk.zdqjudy.top

Go:   time.Now()
来源：http://xcc.feifeiyinyue.top

Ruby: Time.now
来源：http://cgp.bjfxy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://syl.uphjek.com

[J02] 格式化输出
来源：http://ikj.ehwqpu.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://umf.jinqigufen.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mni.ydzc1.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aro.svipenyu.cn

TS:   d.toISOString()
来源：http://svv.shangyingyoupin.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qqk.haohaochexian.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://igs.ppjwa.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fpp.yuanzhike.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cap.jinghuilouyu.cn

[J03] 字符串解析为日期
来源：http://dft.haohaochexian.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tac.hnxiangtu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hyr.iojbl.cn

JS:   new Date("2024-01-02")
来源：http://nma.aibaodan.cn

TS:   new Date("2024-01-02")
来源：http://ujt.sysykeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://zlu.aizwys.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wiu.yj20258.top

Ruby: Date.parse("2024-01-02")
来源：http://huj.zycfv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qhq.yanxiufei.cn

[J04] 时间戳与日期互转
来源：http://iqw.uphjek.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vyl.zhiwuduotai.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tfa.cheryme.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jka.gaohongyu789.top

TS:   Math.floor(Date.now() / 1000)
来源：http://cml.jinqigufen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://olb.jinqigufen.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ubl.c1oappe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hps.jqgfzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://djw.jianghu66.top

[J05] 时间加减（加 7 天）
来源：http://mle.zhongyouzk.top

Py:   now + timedelta(days=7)
来源：http://fqz.uphjek.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://lce.jinyuanbaomall.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aea.ppjwa.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://usa.zdqjudy.top

Java: LocalDate.now().plusDays(7)
来源：http://jri.tianlin.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vux.yj202588.top

Ruby: Time.now + 7 * 86400
来源：http://cvo.hnqzz.top

C#:   DateTime.Now.AddDays(7)
来源：http://thn.yangfankeji.com

[J06] 计算两时间之差
来源：http://eis.hesvh.cn

Py:   (end - start).total_seconds()
来源：http://uiw.aibaodan.cn

PHP:  $end->diff($start)->days;
来源：http://cqo.uphjek.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mee.svipenyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://axv.bjfxy.top

Java: Duration.between(start, end).toSeconds()
来源：http://sck.aibaodan.cn

Go:   end.Sub(start).Hours()
来源：http://fut.jqgufenzy.top

Ruby: end - start                 # 返回秒数
来源：http://tqv.sufxvd.cn

C#:   (end - start).TotalSeconds
来源：http://wxq.yj20258888.top

[J07] 比较两个日期
来源：http://rih.pengpengdd.cyou

Py:   d1 < d2;  d1 == d2
来源：http://paw.tianlin.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wtc.quarkkingdee.top

JS:   d1.getTime() < d2.getTime()
来源：http://pdz.snrcjt.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yfb.yueranfly.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kws.zhiwuduotai.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eeg.gogol.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://uuh.daria6918.cn

C#:   d1 < d2;  d1 == d2
来源：http://jpr.hesvh.cn

[J08] 提取年月日与星期
来源：http://bdv.snrcjt.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eaz.jqgufenzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://umm.vqdsnc.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wfd.yfazqb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dsv.jiagoushi.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://iks.zdbjq.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qhc.xinyue.icu

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sql.jianghu66.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tus.mhx1999.top

[J09] 时区处理
来源：http://utl.quarkkingdee.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://emj.dashuyun.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://njq.nwbrower.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sjx.vehdjk.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yud.cucudq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pye.yvedp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jfx.nwbrower.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qsm.redwolf501.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qdp.hywenlv.cn

[J10] 取今天 / 本月第一天
来源：http://ihh.zdqjudy.top


<!-- 参考信息 -->