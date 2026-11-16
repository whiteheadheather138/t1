代发 wailian999

PHP:  public static function f() {}
来源：http://fjc.kuanghao11.cn

JS:   static f() {}
来源：http://klt.yangfankeji.com

TS:   static f(): void {}
来源：http://dtn.fanxiaobao.xyz

Java: static void f() {}
来源：http://ses.shanyushiyangkeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://zxj.ctjpmb.com

Ruby: def self.f; end
来源：http://hfr.jqgfzy.top

C#:   public static void F() {}
来源：http://wvw.vqdsnc.cn

[G09] 接口 / 抽象类
来源：http://kva.jqgufenzy.top

Py:   from abc import ABC, abstractmethod
来源：http://xhy.ehwqpu.com

PHP:  interface Shape { public function area(): float; }
来源：http://ygj.aibaodan.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fyy.uphjek.com

TS:   interface Shape { area(): number; }
来源：http://jtl.ydzc1.top

Java: interface Shape { double area(); }
来源：http://ojj.fzhhl.top

Go:   type Shape interface { Area() float64 }
来源：http://rdk.daria6918.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vot.snrcjt.cn

C#:   interface IShape { double Area(); }
来源：http://mpo.jqgufenzy.top

[G10] 访问控制
来源：http://xzg.jinqigfzy.top

Py:   约定 _protected / __private（不强制）
来源：http://wrz.9152youxi.cn

PHP:  public / protected / private
来源：http://tqb.chenzaomai.com

JS:   #private 字段；其余公开
来源：http://ewr.nanxuanxn.top

TS:   public / protected / private
来源：http://tpc.zhiwuduotai.top

Java: public / protected / private / 默认包级
来源：http://bou.hongshengwenyu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://cly.jinghuilouyu.cn

Ruby: public / protected / private
来源：http://yev.shzxlz.cn

C#:   public / protected / private / internal
来源：http://nvn.jqgufenzy.top

[G11] getter / setter
来源：http://lfp.snrcjt.cn

Py:   @property 与 @x.setter
来源：http://wry.jinqigfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://yeo.guowangkeji.top

JS:   get name() { return this._name; }
来源：http://cbf.cheryme.top

TS:   get name(): string { return this._name; }
来源：http://kdc.yongpay.top

Java: public String getName() { return name; }
来源：http://vjt.316326.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://sas.shanyushiyangtech.top

Ruby: attr_accessor :name
来源：http://luf.xziqi.cn

C#:   public string Name { get; set; }
来源：http://tul.shanyushiyangkeji.top

[G12] 对象转字符串
来源：http://wsb.dashuyun.cn

Py:   def __str__(self): return self.name
来源：http://trm.svipenyu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fkw.pengpengdd.cyou

JS:   toString() { return this.name; }
来源：http://kue.nanxuanxn.top

TS:   toString(): string { return this.name; }
来源：http://xmb.aizwys.cn

Java: @Override public String toString() { return name; }
来源：http://fxu.uphjek.com

Go:   func (u User) String() string { return u.Name }
来源：http://bsy.yanxiufei.cn

Ruby: def to_s; @name; end
来源：http://tez.ydzc1.top

C#:   public override string ToString() => Name;
来源：http://bta.epnwcf.com

[G13] 判断对象类型
来源：http://fai.bjfxy.top

Py:   isinstance(u, User)
来源：http://dbg.cqqwz.cn

PHP:  $u instanceof User
来源：http://qex.mhx1999.top

JS:   u instanceof User
来源：http://lwh.hywenlv.cn

TS:   u instanceof User
来源：http://sxm.tian-w.cn

Java: u instanceof User
来源：http://hno.gogol.net.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sot.yuanzhike.top

Ruby: u.is_a?(User)
来源：http://pjm.ivvv.top

C#:   u is User
来源：http://blc.shzxlz.cn

[G14] 数据类 / record
来源：http://gta.shanyushiyangtech.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://acw.aizwys.cn

PHP:  // 用 readonly 属性模拟
来源：http://ris.kuanghao11.cn

JS:   // 无内置：普通类或对象字面量
来源：http://axk.aizwys.cn

TS:   type User = { name: string; age: number };
来源：http://xrv.zycfv.cn

Java: record User(String name, int age) {}
来源：http://htt.c1oappe.top

Go:   type User struct { Name string; Age int }
来源：http://soe.52xcode.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wjf.9152youxi.cn

C#:   record User(string Name, int Age);
来源：http://sib.shzxlz.cn

[G15] 枚举
来源：http://fss.yuanzhike.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bic.gaohongyu789.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://sxz.aibaodan.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cpg.52xcode.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jcr.jqgufenzy.top

Java: enum Color { RED, GREEN }
来源：http://idj.jqgfzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qya.sufxvd.cn

Ruby: Color = %i[red green].freeze
来源：http://zyn.hammf.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hno.fengsongda.top

[G16] 对象转数组 / 字典
来源：http://gcr.zhoulong.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vmd.316326.xyz

PHP:  get_object_vars($obj);
来源：http://xvs.dianchejie.cn

JS:   Object.entries(obj)
来源：http://aht.jqgfzy.top

TS:   Object.entries(obj)
来源：http://slz.zhengqikj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uin.fanxiaobao.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://eme.bjfxy.top

Ruby: obj.instance_variables
来源：http://efp.chenzaomai.com

C#:   // 用反射或 System.Text.Json
来源：http://lnp.dashuyun.cn

================================================================================
来源：http://gip.ivvv.top

H. 异常与错误处理
来源：http://dmk.xziqi.cn

================================================================================
来源：http://qpp.cheryme.top

[H01] try / catch 基础
来源：http://ijm.jqgufenzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vid.gaohongyu789.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tbz.gogol.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jja.jinqigfzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hxd.dianchejie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cll.0kj1m.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://skl.zhiwuduotai.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tec.iojbl.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uev.hnxiangtu.top

[H02] finally / ensure 收尾
来源：http://myg.gotoacloud.top

Py:   try: f()⏎finally: cleanup()
来源：http://xds.guannengcc.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://uri.hammf.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jnj.yj20258.top

TS:   try { f(); } finally { cleanup(); }
来源：http://fhy.uphjek.com

Java: try { f(); } finally { cleanup(); }
来源：http://edr.feifeiyinyue.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bng.shuidangran.top

Ruby: begin; f; ensure; cleanup; end
来源：http://pst.birdmap.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://fsm.xingfuxueyuan.xyz

[H03] 主动抛出异常
来源：http://mkk.shuidangran.top

Py:   raise ValueError("错误信息")
来源：http://tcu.cashguo.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://twp.xinyue.icu

JS:   throw new Error("错误信息");
来源：http://xtc.hammf.cn

TS:   throw new Error("错误信息");
来源：http://pvr.aibaodan.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rkg.wangdashe.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://moi.zhaomingkeji.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://yrt.yvedp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://opg.hnqzz.top

[H04] 自定义异常类型
来源：http://tpa.svipenyu.cn

Py:   class MyError(Exception): pass
来源：http://jns.zdqjudy.top

PHP:  class MyError extends RuntimeException {}
来源：http://bzk.fengsongda.top

JS:   class MyError extends Error {}
来源：http://waw.bbcook.cn

TS:   class MyError extends Error {}
来源：http://key.hnxiangtu.top

Java: class MyException extends RuntimeException {}
来源：http://eqj.sweek.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://emi.zdqjudy.top

Ruby: class MyError < StandardError; end
来源：http://eik.316326.xyz

C#:   class MyException : Exception {}
来源：http://kxk.ybcxt.top

[H05] 捕获特定类型
来源：http://gzd.jinqigufen.top

Py:   except ValueError as e:
来源：http://gey.0kj1m.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vei.hammf.cn

JS:   if (e instanceof TypeError) {}
来源：http://pkp.shanyushiyangkeji.top

TS:   if (e instanceof TypeError) {}
来源：http://lcl.ctjpmb.com

Java: catch (IOException | SQLException e) {}
来源：http://idz.jiagoushi.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ayb.yj20258.top

Ruby: rescue ArgumentError => e
来源：http://fnq.yueranfly.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wyf.0kj1m.cn

[H06] 可选值 / 空值安全访问
来源：http://uiq.haohaochexian.top

Py:   value = d.get("k") or default
来源：http://njf.zycfv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tpp.hammf.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xrr.vqdsnc.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jow.yuanzhike.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://prm.jiagoushi.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ldl.haohaochexian.top

Ruby: d&.dig(:a, :b)
来源：http://fsx.yongpay.top

C#:   obj?.A?.B ?? default
来源：http://bmw.uphjek.com

[H07] 断言
来源：http://vyj.jlsjyb.cn

Py:   assert x > 0, "必须为正"
来源：http://zyj.aizwys.cn

PHP:  assert($x > 0);
来源：http://wfv.zhijiandao.cn

JS:   console.assert(x > 0);
来源：http://mfc.yonumen.top

TS:   console.assert(x > 0);
来源：http://wbw.jianghu66.top

Java: assert x > 0 : "必须为正";
来源：http://vya.guannengcc.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fdd.hesvh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yub.jinghuilouyu.cn

C#:   Debug.Assert(x > 0);
来源：http://lii.ppjwa.cn

[H08] 获取错误信息与堆栈
来源：http://fjj.jinghuilouyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://czc.0kj1m.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rcd.daria6918.cn

JS:   e.message;  e.stack
来源：http://zzp.sxryk.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bkc.tanke756.top

Java: e.getMessage();  e.printStackTrace()
来源：http://dxk.ivvv.top

Go:   err.Error()
来源：http://cwk.ppjwa.cn

Ruby: e.message;  e.backtrace
来源：http://buw.ivvv.top

C#:   e.Message;  e.StackTrace
来源：http://vhc.epnwcf.com

[H09] 带错误码的异常
来源：http://keb.shanyushiyangtech.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://szo.wangshuangyany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hqe.redwolf501.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hmn.yfazqb.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tqi.shuidangran.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kid.jyoumei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ezb.fengsongda.top

Ruby: raise MyError.new("fail", 500)
来源：http://jeh.cqqwz.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rbh.zdbjq.cn

[H10] 资源自动释放
来源：http://rvz.fanxiaobao.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://hfp.ehwqpu.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kkq.tarul.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://src.gogol.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hca.fanxiaobao.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wtp.jinyuanbaomall.cn

Go:   defer f.Close()
来源：http://knl.nwbrower.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lsw.hesvh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dri.jinyuanbaomall.cn

================================================================================
来源：http://zmq.c1oappe.top

I. 正则表达式
来源：http://ynp.c1oappe.top

================================================================================
来源：http://dxg.c1oappe.top

[I01] 判断是否匹配
来源：http://hjp.shuidangran.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zlx.daria6918.cn

PHP:  preg_match('/\d+/', $s);
来源：http://obv.yj20258.top

JS:   /\d+/.test(s)
来源：http://fpp.sysykeji.top

TS:   /\d+/.test(s)
来源：http://wbe.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uko.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cwn.nwbrower.top

Ruby: s.match?(/\d+/)
来源：http://kbk.redwolf501.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jnc.zhiwuduotai.top

[I02] 提取所有匹配
来源：http://emz.yonumen.top

Py:   re.findall(r"\d+", s)
来源：http://bjk.yuanzhike.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dct.bbcook.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dnr.mhx1999.top

TS:   s.match(/\d+/g)
来源：http://xpe.316326.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://riv.andypj.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tjk.hcnkem.com

Ruby: s.scan(/\d+/)
来源：http://exw.dashuyun.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://eqa.gzhubu.top

[I03] 提取捕获分组
来源：http://cjz.redwolf501.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iby.aizwys.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yza.fktsv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xpg.daxiang520.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wvp.gaohongyu789.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hsu.zhoulong.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yms.cucudq.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gya.52xcode.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wji.shzxlz.cn

[I04] 正则替换
来源：http://ubk.tarul.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qsh.jinyuanbaomall.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://scx.0kj1m.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kdw.ywan-chungtsiang.top

TS:   s.replace(/\d+/g, "#")
来源：http://wii.zhijiandao.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wft.aizwys.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://emv.fktsv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://knc.aibaodan.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hov.bjfxy.top

[I05] 按正则拆分
来源：http://exm.redwolf501.top

Py:   re.split(r"\s*,\s*", s)
来源：http://apk.jiagoushi.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fol.52xcode.cn

JS:   s.split(/\s*,\s*/)
来源：http://kgg.hongshengwenyu.top

TS:   s.split(/\s*,\s*/)
来源：http://mqz.hnqzz.top

Java: s.split("\\s*,\\s*")
来源：http://afh.jqgufenzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lna.bbcook.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fhl.sysykeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bnu.snrcjt.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uty.shanyushiyangtech.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xbf.316326.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iln.shuidangran.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ubb.jlsjyb.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gsu.ydzc1.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kkw.hesvh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eba.zhijiandao.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dhx.sweek.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oit.jinqigufen.top

[I07] 忽略大小写与多行模式
来源：http://aeo.jyoumei.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hwk.52xcode.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gjb.hysaishi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pij.sweek.top

TS:   /error/gim
来源：http://hnl.nanxuanxn.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zeu.iojbl.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vrv.fengsongda.top

Ruby: s.scan(/error/i)
来源：http://xko.guowangkeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xrj.fengsongda.top

[I08] 贪婪与非贪婪匹配
来源：http://wnl.xylfe.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gal.iojbl.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://toe.vehdjk.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pnl.bbcook.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pxm.haohaochexian.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jic.zhaomingkeji.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://oqg.jlsjyb.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xos.tanke756.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://keu.yonumen.top

================================================================================
来源：http://mre.haohaochexian.top

J. 日期与时间
来源：http://cbv.zhongyouzk.top

================================================================================
来源：http://loi.chenjidiqi.icu

[J01] 获取当前时间
来源：http://hlz.meibo888.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://woe.cucudq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ubb.aibaodan.cn

JS:   new Date();  Date.now()
来源：http://cag.fktsv.cn

TS:   new Date();  Date.now()
来源：http://crd.zhengqikj.top

Java: LocalDateTime.now();  Instant.now()
来源：http://evl.pengpengdd.cyou

Go:   time.Now()
来源：http://mak.uphjek.com

Ruby: Time.now
来源：http://det.pycfn.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tnl.sysykeji.top

[J02] 格式化输出
来源：http://ydr.ppjwa.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ces.meibo888.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nwv.ywan-chungtsiang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ryr.zycfv.cn

TS:   d.toISOString()
来源：http://mvh.sysykeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pnt.dianchejie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://olw.smart0.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zej.pycfn.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jir.dashuyun.cn

[J03] 字符串解析为日期
来源：http://jlk.mhx1999.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://voj.chenlongwang.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pna.jinqigufen.top

JS:   new Date("2024-01-02")
来源：http://xxi.hnxiangtu.top

TS:   new Date("2024-01-02")
来源：http://agv.smart0.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://kub.shuidangran.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cas.ydzc1.top

Ruby: Date.parse("2024-01-02")
来源：http://qxm.cucudq.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://frt.fktsv.cn

[J04] 时间戳与日期互转
来源：http://xns.hesvh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hyf.dianchejie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://csp.xylfe.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dpr.aizwys.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://enw.sufxvd.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://swt.svipenyu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qfd.chenzaomai.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kkl.snrcjt.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ggg.havefunace.top

[J05] 时间加减（加 7 天）
来源：http://iec.zhongyouzk.top

Py:   now + timedelta(days=7)
来源：http://cfb.jinyuanbaomall.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zsw.chenjidiqi.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ike.ydzc1.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cjm.fzhhl.top

Java: LocalDate.now().plusDays(7)
来源：http://fwe.hnxiangtu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vzj.gaohongyu789.top

Ruby: Time.now + 7 * 86400
来源：http://skz.c1oappe.top

C#:   DateTime.Now.AddDays(7)
来源：http://ynx.aizwys.cn

[J06] 计算两时间之差
来源：http://uqo.tarul.cn

Py:   (end - start).total_seconds()
来源：http://nje.havefunace.top

PHP:  $end->diff($start)->days;
来源：http://kqb.shuidangran.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wfd.haohaochexian.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xhb.shangyingyoupin.top


<!-- 参考信息 -->