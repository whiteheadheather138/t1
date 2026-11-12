代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://qwc.hcnkem.com

Ruby: def self.f; end
来源：http://svi.gotoacloud.top

C#:   public static void F() {}
来源：http://sso.tanke756.top

[G09] 接口 / 抽象类
来源：http://sij.xinyue.icu

Py:   from abc import ABC, abstractmethod
来源：http://pka.cheryme.top

PHP:  interface Shape { public function area(): float; }
来源：http://hti.shzxlz.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nxp.ybcxt.top

TS:   interface Shape { area(): number; }
来源：http://vks.quarkkingdee.top

Java: interface Shape { double area(); }
来源：http://ksy.hammf.cn

Go:   type Shape interface { Area() float64 }
来源：http://qmo.zhixingplan.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oad.zhongyouzk.top

C#:   interface IShape { double Area(); }
来源：http://yet.ybcxt.top

[G10] 访问控制
来源：http://pgp.guowangkeji.top

Py:   约定 _protected / __private（不强制）
来源：http://wiy.sufxvd.cn

PHP:  public / protected / private
来源：http://pjd.jinyuanbaomall.cn

JS:   #private 字段；其余公开
来源：http://bay.ehwqpu.com

TS:   public / protected / private
来源：http://lvi.xziqi.cn

Java: public / protected / private / 默认包级
来源：http://dft.bjfxy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://pme.yj20258.top

Ruby: public / protected / private
来源：http://lqg.hongshengwenyu.top

C#:   public / protected / private / internal
来源：http://bve.shanyushiyangtech.top

[G11] getter / setter
来源：http://otw.kuanghao11.cn

Py:   @property 与 @x.setter
来源：http://zvq.fktsv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://aih.zdqjudy.top

JS:   get name() { return this._name; }
来源：http://yev.jlsjyb.cn

TS:   get name(): string { return this._name; }
来源：http://uln.ppjwa.cn

Java: public String getName() { return name; }
来源：http://rzf.ydzc1.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://qgq.xinyue.icu

Ruby: attr_accessor :name
来源：http://spg.zhaomingkeji.xyz

C#:   public string Name { get; set; }
来源：http://qtv.cqqwz.cn

[G12] 对象转字符串
来源：http://gwa.zhixingplan.top

Py:   def __str__(self): return self.name
来源：http://bkb.zhiwuduotai.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://sjm.hnqzz.top

JS:   toString() { return this.name; }
来源：http://uxo.guannengcc.top

TS:   toString(): string { return this.name; }
来源：http://nfm.guannengcc.top

Java: @Override public String toString() { return name; }
来源：http://luj.quarkkingdee.top

Go:   func (u User) String() string { return u.Name }
来源：http://iqd.jqgufenzy.top

Ruby: def to_s; @name; end
来源：http://xwe.bjfxy.top

C#:   public override string ToString() => Name;
来源：http://wyo.nwbrower.top

[G13] 判断对象类型
来源：http://gqa.fktsv.cn

Py:   isinstance(u, User)
来源：http://spf.hfpthk.cn

PHP:  $u instanceof User
来源：http://acn.yj20258888.top

JS:   u instanceof User
来源：http://qux.zhiwuduotai.top

TS:   u instanceof User
来源：http://qhm.sufxvd.cn

Java: u instanceof User
来源：http://ihb.jyoumei.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mdo.jinyuanbaomall.cn

Ruby: u.is_a?(User)
来源：http://blp.ehwqpu.com

C#:   u is User
来源：http://fxh.chenlongwang.top

[G14] 数据类 / record
来源：http://imb.nwbrower.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fzm.hnxiangtu.top

PHP:  // 用 readonly 属性模拟
来源：http://ifp.jianghu66.top

JS:   // 无内置：普通类或对象字面量
来源：http://cxg.hongshengwenyu.top

TS:   type User = { name: string; age: number };
来源：http://arg.jinqigufen.top

Java: record User(String name, int age) {}
来源：http://cth.yj202588.top

Go:   type User struct { Name string; Age int }
来源：http://oby.xziqi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kaq.havefunace.top

C#:   record User(string Name, int Age);
来源：http://nly.sjlbkw.cn

[G15] 枚举
来源：http://tfp.sjlbkw.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nbm.shanyushiyangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://hrh.svipenyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sgt.havefunace.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://oph.vehdjk.com

Java: enum Color { RED, GREEN }
来源：http://cii.jiagoushi.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lbw.xziqi.cn

Ruby: Color = %i[red green].freeze
来源：http://rsw.vehdjk.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://upn.meibo888.top

[G16] 对象转数组 / 字典
来源：http://ngb.yuxming.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zyx.yuxming.cn

PHP:  get_object_vars($obj);
来源：http://qkt.hywenlv.cn

JS:   Object.entries(obj)
来源：http://rgr.ydjk.org.cn

TS:   Object.entries(obj)
来源：http://pqd.zhijiandao.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mra.uphjek.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://mdl.xylfe.cn

Ruby: obj.instance_variables
来源：http://eys.yj20258.top

C#:   // 用反射或 System.Text.Json
来源：http://vpv.hnxiangtu.top

================================================================================
来源：http://pyp.zycfv.cn

H. 异常与错误处理
来源：http://qht.cdnleiting.top

================================================================================
来源：http://kkw.ivvv.top

[H01] try / catch 基础
来源：http://dfs.yongpay.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xrs.nanxuanxn.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cdi.jinghuilouyu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sbi.pycfn.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oqq.zhoulong.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jhs.uphjek.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vnh.redwolf501.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://daf.yj202588.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tnl.316326.xyz

[H02] finally / ensure 收尾
来源：http://qmv.zhengqikj.top

Py:   try: f()⏎finally: cleanup()
来源：http://uyw.shanyushiyangtech.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qmw.hnxiangtu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vgu.iojbl.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tjs.meibo888.top

Java: try { f(); } finally { cleanup(); }
来源：http://bvd.zhaomingkeji.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://wmq.xylfe.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mhi.meibo888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://rhm.chenlongwang.top

[H03] 主动抛出异常
来源：http://tgy.nanxuanxn.top

Py:   raise ValueError("错误信息")
来源：http://prz.fzhhl.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mjx.hnxiangtu.top

JS:   throw new Error("错误信息");
来源：http://mde.fktsv.cn

TS:   throw new Error("错误信息");
来源：http://qen.jianghu66.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://rxo.bbcook.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hef.yanxiufei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rmm.ywan-chungtsiang.top

C#:   throw new ArgumentException("错误信息");
来源：http://cdy.yj20258.top

[H04] 自定义异常类型
来源：http://esj.havefunace.top

Py:   class MyError(Exception): pass
来源：http://apb.fktsv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ukz.hnxiangtu.top

JS:   class MyError extends Error {}
来源：http://njd.jyoumei.cn

TS:   class MyError extends Error {}
来源：http://hnp.sjlbkw.cn

Java: class MyException extends RuntimeException {}
来源：http://sxe.zhaomingkeji.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nbv.cqqwz.cn

Ruby: class MyError < StandardError; end
来源：http://hkf.yj202588.top

C#:   class MyException : Exception {}
来源：http://ncz.shanyushiyangtech.top

[H05] 捕获特定类型
来源：http://grl.ehwqpu.com

Py:   except ValueError as e:
来源：http://dfn.hongshengwenyu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mou.ywan-chungtsiang.top

JS:   if (e instanceof TypeError) {}
来源：http://zkb.tarul.cn

TS:   if (e instanceof TypeError) {}
来源：http://esu.meibo888.top

Java: catch (IOException | SQLException e) {}
来源：http://vyq.jyoumei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lej.yangfankeji.com

Ruby: rescue ArgumentError => e
来源：http://esk.pengpengdd.cyou

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://igy.snrcjt.cn

[H06] 可选值 / 空值安全访问
来源：http://pns.smart0.xyz

Py:   value = d.get("k") or default
来源：http://osr.c1oappe.top

PHP:  $v = $d["k"] ?? null;
来源：http://wwg.fehbvm.com

JS:   obj?.a?.b;  d ?? default
来源：http://mgr.zhongyouzk.top

TS:   obj?.a?.b;  d ?? default
来源：http://hwh.cqqwz.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ljo.gzhubu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://cah.cdnleiting.top

Ruby: d&.dig(:a, :b)
来源：http://olm.jqgufenzy.top

C#:   obj?.A?.B ?? default
来源：http://mrb.zdqjudy.top

[H07] 断言
来源：http://lxu.shangyingyoupin.top

Py:   assert x > 0, "必须为正"
来源：http://bzd.nanxuanxn.top

PHP:  assert($x > 0);
来源：http://fei.9152youxi.cn

JS:   console.assert(x > 0);
来源：http://xrw.aibaodan.cn

TS:   console.assert(x > 0);
来源：http://cfy.daria6918.cn

Java: assert x > 0 : "必须为正";
来源：http://fll.yj20258888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qnv.tianlin.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://cpn.hywenlv.cn

C#:   Debug.Assert(x > 0);
来源：http://nau.dashuyun.cn

[H08] 获取错误信息与堆栈
来源：http://hei.xziqi.cn

Py:   str(e);  traceback.format_exc()
来源：http://taa.yanxiufei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sic.xylfe.cn

JS:   e.message;  e.stack
来源：http://tqm.sufxvd.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://spo.gaohongyu789.top

Java: e.getMessage();  e.printStackTrace()
来源：http://fpb.zhengqikj.top

Go:   err.Error()
来源：http://man.yanxiufei.cn

Ruby: e.message;  e.backtrace
来源：http://vwz.vqdsnc.cn

C#:   e.Message;  e.StackTrace
来源：http://yge.jinqigufen.top

[H09] 带错误码的异常
来源：http://izr.svipenyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yns.smart0.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://igm.yanxiufei.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vwv.yuanzhike.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gpq.aibaodan.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nsj.jinyuanbaomall.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bhz.wangshuangyany.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mlx.xuanzx.com

C#:   // 自定义异常类中加 Code 属性
来源：http://wpx.tanke756.top

[H10] 资源自动释放
来源：http://dda.chenlongwang.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ngg.hongshengwenyu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://usj.chenjidiqi.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://klc.yuxming.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gik.dianchejie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xjk.0kj1m.cn

Go:   defer f.Close()
来源：http://pog.gzhubu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zyf.hesvh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://urq.zycfv.cn

================================================================================
来源：http://ddi.yfazqb.com

I. 正则表达式
来源：http://rku.shuidangran.top

================================================================================
来源：http://gqs.smart0.xyz

[I01] 判断是否匹配
来源：http://slc.zhixingplan.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lsh.iojbl.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zmy.chenzaomai.com

JS:   /\d+/.test(s)
来源：http://bdx.zhoulong.xyz

TS:   /\d+/.test(s)
来源：http://nlf.tian-w.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eqj.yuxming.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://djl.yj20258888.top

Ruby: s.match?(/\d+/)
来源：http://xsq.xuetiantiany.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ury.nwbrower.top

[I02] 提取所有匹配
来源：http://nzt.sysykeji.top

Py:   re.findall(r"\d+", s)
来源：http://hnr.smart0.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://niv.jqgfzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kvo.guannengcc.top

TS:   s.match(/\d+/g)
来源：http://bnm.haohaochexian.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gnm.jianghu66.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vle.shzxlz.cn

Ruby: s.scan(/\d+/)
来源：http://pfq.bbcook.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qce.zdqjudy.top

[I03] 提取捕获分组
来源：http://tnq.guannengcc.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uss.chenlongwang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sqj.xuanzx.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gug.svipenyu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pga.52xcode.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qrf.ehwqpu.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pld.vqdsnc.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://npd.hammf.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cqa.xingfuxueyuan.xyz

[I04] 正则替换
来源：http://dyd.guowangkeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://civ.vehdjk.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://idd.jinqigfzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://zrd.vehdjk.com

TS:   s.replace(/\d+/g, "#")
来源：http://jbz.pycfn.com

Java: s.replaceAll("\\d+", "#")
来源：http://pbg.jinghuilouyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lmt.jinqigufen.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qwh.hnxiangtu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://njc.zhengqikj.top

[I05] 按正则拆分
来源：http://qbv.yangfankeji.com

Py:   re.split(r"\s*,\s*", s)
来源：http://nta.gzhubu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://igh.gogol.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://vni.mhx1999.top

TS:   s.split(/\s*,\s*/)
来源：http://ueh.fzhhl.top

Java: s.split("\\s*,\\s*")
来源：http://loy.pengpengdd.cyou

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kqh.shuidangran.top

Ruby: s.split(/\s*,\s*/)
来源：http://rib.9152youxi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ihx.tanke756.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xaj.yangfankeji.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ume.9152youxi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kzo.birdmap.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zxc.316326.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mym.nanxinkj.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://abq.ydzc1.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fgv.zhengqikj.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ueb.chenlongwang.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lkk.sjlbkw.cn

[I07] 忽略大小写与多行模式
来源：http://vcn.guannengcc.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sue.ctjpmb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cpj.guowangkeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dru.fengsongda.top

TS:   /error/gim
来源：http://lri.jlsjyb.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qtb.cdnleiting.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://auq.ywan-chungtsiang.top

Ruby: s.scan(/error/i)
来源：http://kho.epnwcf.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pqn.hysaishi.cn

[I08] 贪婪与非贪婪匹配
来源：http://wvw.jianghu66.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pzt.nanxinkj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xgd.sweek.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bfk.zhengqikj.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xev.xylfe.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://drs.shuidangran.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pkc.shuidangran.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rwl.bjfxy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hyv.zycfv.cn

================================================================================
来源：http://uyg.fanxiaobao.xyz

J. 日期与时间
来源：http://uxz.cdnleiting.top

================================================================================
来源：http://blu.ybcxt.top

[J01] 获取当前时间
来源：http://obs.hesvh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bmx.jqgfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bmb.jinyuanbaomall.cn

JS:   new Date();  Date.now()
来源：http://skh.uphjek.com

TS:   new Date();  Date.now()
来源：http://gca.birdmap.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ihj.guowangkeji.top

Go:   time.Now()
来源：http://kgs.zhijiandao.cn

Ruby: Time.now
来源：http://qxm.yueranfly.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://eye.dianchejie.cn

[J02] 格式化输出
来源：http://nzv.zhengqikj.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://twb.hywenlv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dul.chenzaomai.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://axx.svipenyu.cn

TS:   d.toISOString()
来源：http://uyx.zhijiandao.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rtw.xylfe.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lxo.nwbrower.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jfm.shuidangran.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://klc.zhiwuduotai.top

[J03] 字符串解析为日期
来源：http://yue.tian-w.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ozt.gotoacloud.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vvf.iojbl.cn

JS:   new Date("2024-01-02")
来源：http://vpf.zdqjudy.top

TS:   new Date("2024-01-02")
来源：http://dag.sweek.top

Java: LocalDate.parse("2024-01-02")
来源：http://vsl.ppjwa.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fdk.dianchejie.cn

Ruby: Date.parse("2024-01-02")
来源：http://djr.sxryk.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qjn.yj20258.top

[J04] 时间戳与日期互转
来源：http://cvg.yj202588.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lub.jinqigfzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xyk.ywan-chungtsiang.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ntl.jinghuilouyu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xlr.yj20258.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ypn.bjfxy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xbu.kuanghao11.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qvf.yuanzhike.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cdl.andypj.xyz

[J05] 时间加减（加 7 天）
来源：http://ads.kuanghao11.cn

Py:   now + timedelta(days=7)
来源：http://yhd.yangfankeji.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://twa.gogol.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lii.haohaochexian.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://umr.tanke756.top

Java: LocalDate.now().plusDays(7)
来源：http://srz.wangdashe.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://shy.sxryk.cn

Ruby: Time.now + 7 * 86400
来源：http://uap.chenjidiqi.icu

C#:   DateTime.Now.AddDays(7)
来源：http://gnw.52xcode.cn

[J06] 计算两时间之差
来源：http://smb.yueranfly.top

Py:   (end - start).total_seconds()
来源：http://kdz.quarkkingdee.top

PHP:  $end->diff($start)->days;
来源：http://zht.jinyuanbaomall.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://umj.jinqigufen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vgw.meibo888.top

Java: Duration.between(start, end).toSeconds()
来源：http://hla.cqqwz.cn

Go:   end.Sub(start).Hours()
来源：http://ieq.fktsv.cn

Ruby: end - start                 # 返回秒数
来源：http://bii.gogol.net.cn

C#:   (end - start).TotalSeconds
来源：http://pon.jlsjyb.cn


<!-- 参考信息 -->