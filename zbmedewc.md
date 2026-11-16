代发 wailian999

TS:   public / protected / private
来源：http://uux.zdqjudy.top

Java: public / protected / private / 默认包级
来源：http://omc.jinghuilouyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ile.nanxinkj.top

Ruby: public / protected / private
来源：http://djb.zhoulong.xyz

C#:   public / protected / private / internal
来源：http://gxy.daria6918.cn

[G11] getter / setter
来源：http://pcb.cucudq.cn

Py:   @property 与 @x.setter
来源：http://djd.gzhubu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ntb.ywan-chungtsiang.top

JS:   get name() { return this._name; }
来源：http://hpx.zycfv.cn

TS:   get name(): string { return this._name; }
来源：http://otl.zdqjudy.top

Java: public String getName() { return name; }
来源：http://jip.shuidangran.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://vub.hammf.cn

Ruby: attr_accessor :name
来源：http://tgf.aizwys.cn

C#:   public string Name { get; set; }
来源：http://tsl.jinghuilouyu.cn

[G12] 对象转字符串
来源：http://bpx.yuxming.cn

Py:   def __str__(self): return self.name
来源：http://efb.vqdsnc.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kqa.cashguo.top

JS:   toString() { return this.name; }
来源：http://gjw.cdnleiting.top

TS:   toString(): string { return this.name; }
来源：http://euc.hywenlv.cn

Java: @Override public String toString() { return name; }
来源：http://zks.gaohongyu789.top

Go:   func (u User) String() string { return u.Name }
来源：http://xha.zdbjq.cn

Ruby: def to_s; @name; end
来源：http://uta.andypj.xyz

C#:   public override string ToString() => Name;
来源：http://nno.hfpthk.cn

[G13] 判断对象类型
来源：http://orq.tanke756.top

Py:   isinstance(u, User)
来源：http://ozb.cheryme.top

PHP:  $u instanceof User
来源：http://ove.kuanghao11.cn

JS:   u instanceof User
来源：http://ybk.jinqigfzy.top

TS:   u instanceof User
来源：http://oho.9152youxi.cn

Java: u instanceof User
来源：http://fwt.jiagoushi.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://qkb.sjlbkw.cn

Ruby: u.is_a?(User)
来源：http://hjt.pengpengdd.cyou

C#:   u is User
来源：http://ghr.yonumen.top

[G14] 数据类 / record
来源：http://pey.jlsjyb.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oof.fehbvm.com

PHP:  // 用 readonly 属性模拟
来源：http://fcg.cheryme.top

JS:   // 无内置：普通类或对象字面量
来源：http://cic.ybcxt.top

TS:   type User = { name: string; age: number };
来源：http://gvo.jqgufenzy.top

Java: record User(String name, int age) {}
来源：http://vwt.hongshengwenyu.top

Go:   type User struct { Name string; Age int }
来源：http://ujh.jqgufenzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rsi.tian-w.cn

C#:   record User(string Name, int Age);
来源：http://yzr.zhoulong.xyz

[G15] 枚举
来源：http://mdw.fanxiaobao.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ndk.quarkkingdee.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://wtj.guowangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://msp.cqqwz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cen.wangshuangyany.cn

Java: enum Color { RED, GREEN }
来源：http://poq.quarkkingdee.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://skh.ybcxt.top

Ruby: Color = %i[red green].freeze
来源：http://acs.jyoumei.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kig.iojbl.cn

[G16] 对象转数组 / 字典
来源：http://vpu.c1oappe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cqp.zhongyouzk.top

PHP:  get_object_vars($obj);
来源：http://uvj.yuanzhike.top

JS:   Object.entries(obj)
来源：http://sul.birdmap.top

TS:   Object.entries(obj)
来源：http://jgd.hysaishi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pto.zhijiandao.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://okj.0kj1m.cn

Ruby: obj.instance_variables
来源：http://psv.yj20258.top

C#:   // 用反射或 System.Text.Json
来源：http://wqw.yj20258888.top

================================================================================
来源：http://jov.yvedp.cn

H. 异常与错误处理
来源：http://qfw.tanke756.top

================================================================================
来源：http://vne.xuanzx.com

[H01] try / catch 基础
来源：http://wnk.dianchejie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kiy.dianchejie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ial.iojbl.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wbm.zhijiandao.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bod.guowangkeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://llu.kuanghao11.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tdc.jiagoushi.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ymh.pengpengdd.cyou

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vbi.hysaishi.cn

[H02] finally / ensure 收尾
来源：http://fcw.chenlongwang.top

Py:   try: f()⏎finally: cleanup()
来源：http://yry.birdmap.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fpo.daria6918.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yot.sweek.top

TS:   try { f(); } finally { cleanup(); }
来源：http://kmk.gotoacloud.top

Java: try { f(); } finally { cleanup(); }
来源：http://rrx.ppjwa.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://isa.yj20258.top

Ruby: begin; f; ensure; cleanup; end
来源：http://wqa.mhx1999.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://rgu.vqdsnc.cn

[H03] 主动抛出异常
来源：http://vpp.jqgufenzy.top

Py:   raise ValueError("错误信息")
来源：http://ols.shzxlz.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gbn.shangyingyoupin.top

JS:   throw new Error("错误信息");
来源：http://tch.nanxinkj.top

TS:   throw new Error("错误信息");
来源：http://esw.yvedp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://uas.hysaishi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ypv.hysaishi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ysd.dashuyun.cn

C#:   throw new ArgumentException("错误信息");
来源：http://njk.shanyushiyangkeji.top

[H04] 自定义异常类型
来源：http://rcg.jinqigfzy.top

Py:   class MyError(Exception): pass
来源：http://osq.yj20258.top

PHP:  class MyError extends RuntimeException {}
来源：http://rld.zhiwuduotai.top

JS:   class MyError extends Error {}
来源：http://bmz.dashuyun.cn

TS:   class MyError extends Error {}
来源：http://ayt.fzhhl.top

Java: class MyException extends RuntimeException {}
来源：http://uqy.iojbl.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xet.nwbrower.top

Ruby: class MyError < StandardError; end
来源：http://qcn.nanxuanxn.top

C#:   class MyException : Exception {}
来源：http://zji.ydzc1.top

[H05] 捕获特定类型
来源：http://vjp.zycfv.cn

Py:   except ValueError as e:
来源：http://qud.tarul.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ypw.hfpthk.cn

JS:   if (e instanceof TypeError) {}
来源：http://pfo.jyoumei.cn

TS:   if (e instanceof TypeError) {}
来源：http://grf.jqgfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://wtn.bjfxy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wni.bjfxy.top

Ruby: rescue ArgumentError => e
来源：http://nga.tianlin.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ayg.shanyushiyangtech.top

[H06] 可选值 / 空值安全访问
来源：http://uio.fktsv.cn

Py:   value = d.get("k") or default
来源：http://zwh.yfazqb.com

PHP:  $v = $d["k"] ?? null;
来源：http://jzz.tian-w.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tos.jyoumei.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kzx.fehbvm.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rgs.jinqigufen.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qcb.zhongyouzk.top

Ruby: d&.dig(:a, :b)
来源：http://pmu.yvedp.cn

C#:   obj?.A?.B ?? default
来源：http://ril.quarkkingdee.top

[H07] 断言
来源：http://dhw.52xcode.cn

Py:   assert x > 0, "必须为正"
来源：http://oia.sufxvd.cn

PHP:  assert($x > 0);
来源：http://pyv.sjlbkw.cn

JS:   console.assert(x > 0);
来源：http://maz.guannengcc.top

TS:   console.assert(x > 0);
来源：http://ncb.yueranfly.top

Java: assert x > 0 : "必须为正";
来源：http://rhz.smart0.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lpk.fktsv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qwe.chenjidiqi.icu

C#:   Debug.Assert(x > 0);
来源：http://qcp.ehwqpu.com

[H08] 获取错误信息与堆栈
来源：http://fcc.shanyushiyangtech.top

Py:   str(e);  traceback.format_exc()
来源：http://csu.gotoacloud.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uhs.hongshengwenyu.top

JS:   e.message;  e.stack
来源：http://roz.yj202588.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rdx.jinqigufen.top

Java: e.getMessage();  e.printStackTrace()
来源：http://vja.meibo888.top

Go:   err.Error()
来源：http://ojf.ehwqpu.com

Ruby: e.message;  e.backtrace
来源：http://lyr.gotoacloud.top

C#:   e.Message;  e.StackTrace
来源：http://qdg.epnwcf.com

[H09] 带错误码的异常
来源：http://eeg.hesvh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tva.hfpthk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rfr.sysykeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qwr.zhongyouzk.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hnk.fengsongda.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rmp.fanxiaobao.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lbd.0kj1m.cn

Ruby: raise MyError.new("fail", 500)
来源：http://srj.jinqigfzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ziq.0kj1m.cn

[H10] 资源自动释放
来源：http://wlw.wangshuangyany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fwr.yuanzhike.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qzl.yonumen.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gcv.svipenyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ywd.shanyushiyangtech.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nqu.sxryk.cn

Go:   defer f.Close()
来源：http://eqk.fehbvm.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://idq.fktsv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://aro.sufxvd.cn

================================================================================
来源：http://ouo.hammf.cn

I. 正则表达式
来源：http://rgp.vqdsnc.cn

================================================================================
来源：http://dgx.nanxinkj.top

[I01] 判断是否匹配
来源：http://vak.jiagoushi.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ubn.yfazqb.com

PHP:  preg_match('/\d+/', $s);
来源：http://wxg.316326.xyz

JS:   /\d+/.test(s)
来源：http://okz.zhiwuduotai.top

TS:   /\d+/.test(s)
来源：http://ijz.gaohongyu789.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xmj.tanke756.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://eoy.zhaomingkeji.xyz

Ruby: s.match?(/\d+/)
来源：http://urj.9152youxi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xzk.jinqigufen.top

[I02] 提取所有匹配
来源：http://noa.xuetiantiany.cn

Py:   re.findall(r"\d+", s)
来源：http://lem.jinyuanbaomall.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ebp.sufxvd.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pab.jyoumei.cn

TS:   s.match(/\d+/g)
来源：http://rfa.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://une.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jgy.zhiwuduotai.top

Ruby: s.scan(/\d+/)
来源：http://rfi.9152youxi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uvj.jqgufenzy.top

[I03] 提取捕获分组
来源：http://orx.fktsv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uwk.ydzc1.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uqt.tanke756.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wtd.shuidangran.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ybx.hfpthk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lgx.ppjwa.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lyr.jinghuilouyu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dgj.zdqjudy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sfh.ydjk.org.cn

[I04] 正则替换
来源：http://tkl.xuetiantiany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xev.cashguo.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ara.hysaishi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ixz.birdmap.top

TS:   s.replace(/\d+/g, "#")
来源：http://orh.jqgufenzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://edf.zdqjudy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://miw.redwolf501.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xpd.fzhhl.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rbb.zhaomingkeji.xyz

[I05] 按正则拆分
来源：http://cum.shanyushiyangkeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://eae.yj20258888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yfo.yfazqb.com

JS:   s.split(/\s*,\s*/)
来源：http://lvq.zhongyouzk.top

TS:   s.split(/\s*,\s*/)
来源：http://lfk.aizwys.cn

Java: s.split("\\s*,\\s*")
来源：http://pqa.sufxvd.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jzw.fehbvm.com

Ruby: s.split(/\s*,\s*/)
来源：http://xni.zdbjq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pne.xylfe.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pgc.sweek.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rdk.hongshengwenyu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vps.tian-w.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ikp.iojbl.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jyz.jinyuanbaomall.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qgj.yj202588.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jps.zhaomingkeji.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rfc.wangshuangyany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tjc.ywan-chungtsiang.top

[I07] 忽略大小写与多行模式
来源：http://jgl.fehbvm.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nwo.epnwcf.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vns.9152youxi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://seo.ybcxt.top

TS:   /error/gim
来源：http://ckr.nanxuanxn.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kux.yonumen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rlt.hysaishi.cn

Ruby: s.scan(/error/i)
来源：http://hpx.meibo888.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://byk.yonumen.top

[I08] 贪婪与非贪婪匹配
来源：http://yoh.epnwcf.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yjn.fanxiaobao.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ihj.dashuyun.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nkl.yuxming.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ers.yuxming.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://aot.tarul.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gce.hongshengwenyu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kst.chenlongwang.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kdv.ywan-chungtsiang.top

================================================================================
来源：http://omp.zhixingplan.top

J. 日期与时间
来源：http://trg.chenzaomai.com

================================================================================
来源：http://bbp.shanyushiyangtech.top

[J01] 获取当前时间
来源：http://hlm.fktsv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kqv.hammf.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vsq.bbcook.cn

JS:   new Date();  Date.now()
来源：http://tsd.cqqwz.cn

TS:   new Date();  Date.now()
来源：http://uwb.chenlongwang.top

Java: LocalDateTime.now();  Instant.now()
来源：http://qgj.yvedp.cn

Go:   time.Now()
来源：http://ptb.tianlin.xyz

Ruby: Time.now
来源：http://rgb.cdnleiting.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://juf.cdnleiting.top

[J02] 格式化输出
来源：http://zvh.nanxuanxn.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bam.ctjpmb.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qpx.tianlin.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hbp.hammf.cn

TS:   d.toISOString()
来源：http://vaj.vqdsnc.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rhp.aibaodan.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hfr.316326.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iqo.316326.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://abz.zhijiandao.cn

[J03] 字符串解析为日期
来源：http://kbg.chenzaomai.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ree.ydjk.org.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://utl.zhijiandao.cn

JS:   new Date("2024-01-02")
来源：http://gmw.fzhhl.top

TS:   new Date("2024-01-02")
来源：http://fov.birdmap.top

Java: LocalDate.parse("2024-01-02")
来源：http://lse.zhaomingkeji.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wea.ydzc1.top

Ruby: Date.parse("2024-01-02")
来源：http://qgn.fehbvm.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vwq.yj202588.top

[J04] 时间戳与日期互转
来源：http://ulk.tianlin.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rjt.tianlin.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qrp.xinyue.icu

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cox.hnxiangtu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://epy.quarkkingdee.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dyl.ybcxt.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ilp.jinghuilouyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sfy.jqgfzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ojd.zhaomingkeji.xyz

[J05] 时间加减（加 7 天）
来源：http://jcj.xingfuxueyuan.xyz

Py:   now + timedelta(days=7)
来源：http://kbc.xuetiantiany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://app.yongpay.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ids.bjfxy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ckt.yuxming.cn

Java: LocalDate.now().plusDays(7)
来源：http://kqg.yueranfly.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kwa.zdqjudy.top

Ruby: Time.now + 7 * 86400
来源：http://mpt.zhengqikj.top

C#:   DateTime.Now.AddDays(7)
来源：http://tvk.pycfn.com

[J06] 计算两时间之差
来源：http://qoq.ydjk.org.cn

Py:   (end - start).total_seconds()
来源：http://eqi.uphjek.com

PHP:  $end->diff($start)->days;
来源：http://khm.tianlin.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jgd.hesvh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://udt.9152youxi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pbv.haohaochexian.top

Go:   end.Sub(start).Hours()
来源：http://xkf.fanxiaobao.xyz

Ruby: end - start                 # 返回秒数
来源：http://oan.yfazqb.com

C#:   (end - start).TotalSeconds
来源：http://bbz.ctjpmb.com

[J07] 比较两个日期
来源：http://acv.tian-w.cn

Py:   d1 < d2;  d1 == d2
来源：http://yek.cqqwz.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lpi.nwbrower.top

JS:   d1.getTime() < d2.getTime()
来源：http://lzj.dashuyun.cn

TS:   d1.getTime() < d2.getTime()
来源：http://uzt.wangshuangyany.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ffi.xingfuxueyuan.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jic.xinyue.icu

Ruby: d1 < d2;  d1 == d2
来源：http://bbq.zhijiandao.cn

C#:   d1 < d2;  d1 == d2
来源：http://ikp.nanxuanxn.top

[J08] 提取年月日与星期
来源：http://wqs.hammf.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://svn.316326.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://trf.smart0.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nuv.dianchejie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://czh.zdbjq.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lrh.hnxiangtu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ovy.hnqzz.top


<!-- 参考信息 -->