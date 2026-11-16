代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://ocg.hammf.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vqj.gotoacloud.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://wsn.guannengcc.top

TS:   interface Shape { area(): number; }
来源：http://cqe.daxiang520.top

Java: interface Shape { double area(); }
来源：http://izb.zhixingplan.top

Go:   type Shape interface { Area() float64 }
来源：http://gfz.zdqjudy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qlu.sufxvd.cn

C#:   interface IShape { double Area(); }
来源：http://kkg.zhixingplan.top

[G10] 访问控制
来源：http://qxq.zdbjq.cn

Py:   约定 _protected / __private（不强制）
来源：http://kjh.hnxiangtu.top

PHP:  public / protected / private
来源：http://geb.hfpthk.cn

JS:   #private 字段；其余公开
来源：http://vex.gaohongyu789.top

TS:   public / protected / private
来源：http://nwy.hongshengwenyu.top

Java: public / protected / private / 默认包级
来源：http://srf.yanxiufei.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://aaq.hnqzz.top

Ruby: public / protected / private
来源：http://zzn.zdbjq.cn

C#:   public / protected / private / internal
来源：http://jlh.andypj.xyz

[G11] getter / setter
来源：http://ezb.sxryk.cn

Py:   @property 与 @x.setter
来源：http://jnp.yanxiufei.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jro.xuetiantiany.cn

JS:   get name() { return this._name; }
来源：http://nim.zhijiandao.cn

TS:   get name(): string { return this._name; }
来源：http://zpa.sufxvd.cn

Java: public String getName() { return name; }
来源：http://ovy.nanxinkj.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://cbd.pengpengdd.cyou

Ruby: attr_accessor :name
来源：http://ezp.yuanzhike.top

C#:   public string Name { get; set; }
来源：http://xtr.svipenyu.cn

[G12] 对象转字符串
来源：http://qwc.hcnkem.com

Py:   def __str__(self): return self.name
来源：http://qgk.xuetiantiany.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rco.gzhubu.top

JS:   toString() { return this.name; }
来源：http://toy.316326.xyz

TS:   toString(): string { return this.name; }
来源：http://imt.hnxiangtu.top

Java: @Override public String toString() { return name; }
来源：http://baj.zhaomingkeji.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://pjj.ppjwa.cn

Ruby: def to_s; @name; end
来源：http://yfp.zhongyouzk.top

C#:   public override string ToString() => Name;
来源：http://xom.gogol.net.cn

[G13] 判断对象类型
来源：http://puc.guowangkeji.top

Py:   isinstance(u, User)
来源：http://rqi.shuidangran.top

PHP:  $u instanceof User
来源：http://sxj.yfazqb.com

JS:   u instanceof User
来源：http://tfr.daxiang520.top

TS:   u instanceof User
来源：http://kem.snrcjt.cn

Java: u instanceof User
来源：http://oah.uphjek.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://gye.jyoumei.cn

Ruby: u.is_a?(User)
来源：http://yfh.jinqigfzy.top

C#:   u is User
来源：http://fyd.sufxvd.cn

[G14] 数据类 / record
来源：http://mwd.ybcxt.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ncc.daria6918.cn

PHP:  // 用 readonly 属性模拟
来源：http://xga.yuanzhike.top

JS:   // 无内置：普通类或对象字面量
来源：http://llq.jqgfzy.top

TS:   type User = { name: string; age: number };
来源：http://wvn.gaohongyu789.top

Java: record User(String name, int age) {}
来源：http://qxw.hammf.cn

Go:   type User struct { Name string; Age int }
来源：http://fto.quarkkingdee.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kuh.ybcxt.top

C#:   record User(string Name, int Age);
来源：http://hcv.xylfe.cn

[G15] 枚举
来源：http://mbv.epnwcf.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jzh.quarkkingdee.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://caw.yj20258888.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ebg.xziqi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ppm.hongshengwenyu.top

Java: enum Color { RED, GREEN }
来源：http://anw.quarkkingdee.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tjt.havefunace.top

Ruby: Color = %i[red green].freeze
来源：http://xdp.nwbrower.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://abg.c1oappe.top

[G16] 对象转数组 / 字典
来源：http://boa.jqgfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wtz.hcnkem.com

PHP:  get_object_vars($obj);
来源：http://qom.tanke756.top

JS:   Object.entries(obj)
来源：http://bwf.yueranfly.top

TS:   Object.entries(obj)
来源：http://hkz.gogol.net.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zrc.uphjek.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://zvm.nwbrower.top

Ruby: obj.instance_variables
来源：http://squ.yfazqb.com

C#:   // 用反射或 System.Text.Json
来源：http://xnk.yj20258.top

================================================================================
来源：http://oiu.nanxuanxn.top

H. 异常与错误处理
来源：http://mok.daxiang520.top

================================================================================
来源：http://kub.redwolf501.top

[H01] try / catch 基础
来源：http://erj.yongpay.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fuk.ywan-chungtsiang.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sss.ywan-chungtsiang.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nkx.zycfv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://twu.kuanghao11.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nyf.uphjek.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hme.hnxiangtu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://thh.sjlbkw.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wbj.sxryk.cn

[H02] finally / ensure 收尾
来源：http://iot.cashguo.top

Py:   try: f()⏎finally: cleanup()
来源：http://fdo.ybcxt.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://nxp.nanxinkj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vlc.uphjek.com

TS:   try { f(); } finally { cleanup(); }
来源：http://fyq.yueranfly.top

Java: try { f(); } finally { cleanup(); }
来源：http://ujy.jqgfzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mfi.yuanzhike.top

Ruby: begin; f; ensure; cleanup; end
来源：http://tjf.zhoulong.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://htx.hywenlv.cn

[H03] 主动抛出异常
来源：http://hhk.jinyuanbaomall.cn

Py:   raise ValueError("错误信息")
来源：http://lxa.cashguo.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tbi.jlsjyb.cn

JS:   throw new Error("错误信息");
来源：http://agf.zhixingplan.top

TS:   throw new Error("错误信息");
来源：http://zsj.guannengcc.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hnd.hongshengwenyu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lqq.hnxiangtu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://yuq.redwolf501.top

C#:   throw new ArgumentException("错误信息");
来源：http://bsa.ivvv.top

[H04] 自定义异常类型
来源：http://xdd.ybcxt.top

Py:   class MyError(Exception): pass
来源：http://drt.hysaishi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mhs.yfazqb.com

JS:   class MyError extends Error {}
来源：http://lcv.aibaodan.cn

TS:   class MyError extends Error {}
来源：http://dkp.ehwqpu.com

Java: class MyException extends RuntimeException {}
来源：http://vsf.jianghu66.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://duk.shanyushiyangkeji.top

Ruby: class MyError < StandardError; end
来源：http://gmn.zhixingplan.top

C#:   class MyException : Exception {}
来源：http://irr.yanxiufei.cn

[H05] 捕获特定类型
来源：http://sxg.sweek.top

Py:   except ValueError as e:
来源：http://qpu.zhijiandao.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jni.tian-w.cn

JS:   if (e instanceof TypeError) {}
来源：http://fwb.sufxvd.cn

TS:   if (e instanceof TypeError) {}
来源：http://qtd.sxryk.cn

Java: catch (IOException | SQLException e) {}
来源：http://ueu.sjlbkw.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ltq.hongshengwenyu.top

Ruby: rescue ArgumentError => e
来源：http://sla.yuxming.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jdk.birdmap.top

[H06] 可选值 / 空值安全访问
来源：http://akb.zdqjudy.top

Py:   value = d.get("k") or default
来源：http://yzk.bjfxy.top

PHP:  $v = $d["k"] ?? null;
来源：http://mlr.chenlongwang.top

JS:   obj?.a?.b;  d ?? default
来源：http://pqi.sufxvd.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mdb.andypj.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zvw.ppjwa.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hwv.xuetiantiany.cn

Ruby: d&.dig(:a, :b)
来源：http://iqj.fktsv.cn

C#:   obj?.A?.B ?? default
来源：http://wmz.hongshengwenyu.top

[H07] 断言
来源：http://sbe.guannengcc.top

Py:   assert x > 0, "必须为正"
来源：http://vqq.shanyushiyangtech.top

PHP:  assert($x > 0);
来源：http://oiq.jlsjyb.cn

JS:   console.assert(x > 0);
来源：http://mjp.shanyushiyangtech.top

TS:   console.assert(x > 0);
来源：http://nih.chenzaomai.com

Java: assert x > 0 : "必须为正";
来源：http://xwd.tarul.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ruy.dianchejie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://feg.cdnleiting.top

C#:   Debug.Assert(x > 0);
来源：http://ykh.vqdsnc.cn

[H08] 获取错误信息与堆栈
来源：http://njd.pengpengdd.cyou

Py:   str(e);  traceback.format_exc()
来源：http://mcx.chenjidiqi.icu

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://syb.jyoumei.cn

JS:   e.message;  e.stack
来源：http://dmd.shanyushiyangtech.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://umg.birdmap.top

Java: e.getMessage();  e.printStackTrace()
来源：http://fjq.gotoacloud.top

Go:   err.Error()
来源：http://miw.chenlongwang.top

Ruby: e.message;  e.backtrace
来源：http://ebx.fanxiaobao.xyz

C#:   e.Message;  e.StackTrace
来源：http://awv.yuxming.cn

[H09] 带错误码的异常
来源：http://kpv.cucudq.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pbt.cashguo.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://dkv.fehbvm.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ehx.havefunace.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kut.sweek.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ndy.hywenlv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ben.zhongyouzk.top

Ruby: raise MyError.new("fail", 500)
来源：http://dlz.yj202588.top

C#:   // 自定义异常类中加 Code 属性
来源：http://cju.yangfankeji.com

[H10] 资源自动释放
来源：http://urq.hesvh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mhp.yongpay.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mhs.xinyue.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://iqs.aibaodan.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dta.feifeiyinyue.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rww.nanxuanxn.top

Go:   defer f.Close()
来源：http://pdu.yanxiufei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vdg.yangfankeji.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ykm.bjfxy.top

================================================================================
来源：http://hft.shuidangran.top

I. 正则表达式
来源：http://ldk.ctjpmb.com

================================================================================
来源：http://vvq.xuetiantiany.cn

[I01] 判断是否匹配
来源：http://myh.sysykeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fzj.jinyuanbaomall.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hro.shanyushiyangtech.top

JS:   /\d+/.test(s)
来源：http://sxj.xuetiantiany.cn

TS:   /\d+/.test(s)
来源：http://luj.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uzk.ctjpmb.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fbj.hongshengwenyu.top

Ruby: s.match?(/\d+/)
来源：http://yxv.zycfv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://avs.tarul.cn

[I02] 提取所有匹配
来源：http://wqr.jinyuanbaomall.cn

Py:   re.findall(r"\d+", s)
来源：http://uya.hywenlv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wzt.nanxinkj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ish.pengpengdd.cyou

TS:   s.match(/\d+/g)
来源：http://gyj.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://omo.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kyv.cashguo.top

Ruby: s.scan(/\d+/)
来源：http://qtl.bjfxy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vfs.zdbjq.cn

[I03] 提取捕获分组
来源：http://rme.tanke756.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qqx.bbcook.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mnb.shuidangran.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nax.daxiang520.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://afq.epnwcf.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bvo.hesvh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sjr.zdqjudy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cav.dianchejie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://egd.fzhhl.top

[I04] 正则替换
来源：http://poa.zdqjudy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hty.daria6918.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tcx.chenlongwang.top

JS:   s.replace(/\d+/g, "#")
来源：http://tjx.pengpengdd.cyou

TS:   s.replace(/\d+/g, "#")
来源：http://fpz.svipenyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zmi.sufxvd.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://byr.ywan-chungtsiang.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qxl.c1oappe.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uoj.ivvv.top

[I05] 按正则拆分
来源：http://cos.cucudq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qfr.aibaodan.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fnn.hnxiangtu.top

JS:   s.split(/\s*,\s*/)
来源：http://xqk.zhixingplan.top

TS:   s.split(/\s*,\s*/)
来源：http://ezi.meibo888.top

Java: s.split("\\s*,\\s*")
来源：http://jbl.tianlin.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vuc.hnqzz.top

Ruby: s.split(/\s*,\s*/)
来源：http://hly.quarkkingdee.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qts.jinqigufen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ytf.sjlbkw.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gpq.hywenlv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://eke.tarul.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://srw.hammf.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nhr.vehdjk.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nea.aizwys.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lje.jyoumei.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oxn.aibaodan.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tpm.birdmap.top

[I07] 忽略大小写与多行模式
来源：http://bvs.dashuyun.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rxy.jyoumei.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dqa.hammf.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://adh.zdbjq.cn

TS:   /error/gim
来源：http://iuv.ydzc1.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mlw.cashguo.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gka.cucudq.cn

Ruby: s.scan(/error/i)
来源：http://uwa.yangfankeji.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://itr.zdqjudy.top

[I08] 贪婪与非贪婪匹配
来源：http://cxy.hesvh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pxx.aibaodan.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wim.xziqi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kkr.gaohongyu789.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://beb.sweek.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ucx.yj20258888.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vhx.tianlin.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gqs.chenzaomai.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wtb.meibo888.top

================================================================================
来源：http://ova.jinqigfzy.top

J. 日期与时间
来源：http://ycg.316326.xyz

================================================================================
来源：http://wil.vehdjk.com

[J01] 获取当前时间
来源：http://tka.gaohongyu789.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://kop.shanyushiyangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kkb.zdbjq.cn

JS:   new Date();  Date.now()
来源：http://gaa.cdnleiting.top

TS:   new Date();  Date.now()
来源：http://ego.fengsongda.top

Java: LocalDateTime.now();  Instant.now()
来源：http://fqf.sxryk.cn

Go:   time.Now()
来源：http://vzd.ybcxt.top

Ruby: Time.now
来源：http://syl.jyoumei.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kpb.vqdsnc.cn

[J02] 格式化输出
来源：http://hjg.yongpay.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://clh.zycfv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zwh.ydzc1.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sbx.nanxinkj.top

TS:   d.toISOString()
来源：http://qlh.xziqi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jvo.tianlin.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ere.yueranfly.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jmk.yuxming.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rdx.shanyushiyangtech.top

[J03] 字符串解析为日期
来源：http://fdt.hnxiangtu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bho.fktsv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aet.gzhubu.top

JS:   new Date("2024-01-02")
来源：http://kux.xziqi.cn

TS:   new Date("2024-01-02")
来源：http://npe.yuanzhike.top

Java: LocalDate.parse("2024-01-02")
来源：http://ohv.zdqjudy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bzp.zhijiandao.cn

Ruby: Date.parse("2024-01-02")
来源：http://jel.gotoacloud.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gkb.hesvh.cn

[J04] 时间戳与日期互转
来源：http://hlt.9152youxi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ipb.bjfxy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://flk.hfpthk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tsr.cashguo.top

TS:   Math.floor(Date.now() / 1000)
来源：http://akz.pengpengdd.cyou

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://knq.nwbrower.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ufm.zycfv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tnd.zhiwuduotai.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pvp.xuanzx.com

[J05] 时间加减（加 7 天）
来源：http://hod.tanke756.top

Py:   now + timedelta(days=7)
来源：http://pfo.xylfe.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mrf.sufxvd.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ejj.shzxlz.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mqn.birdmap.top

Java: LocalDate.now().plusDays(7)
来源：http://wed.cqqwz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cug.cashguo.top

Ruby: Time.now + 7 * 86400
来源：http://fkd.sysykeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://wav.gzhubu.top

[J06] 计算两时间之差
来源：http://dvx.nanxinkj.top

Py:   (end - start).total_seconds()
来源：http://qpl.jiagoushi.top

PHP:  $end->diff($start)->days;
来源：http://qll.pengpengdd.cyou

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ryx.shanyushiyangtech.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jtl.fanxiaobao.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://qan.316326.xyz

Go:   end.Sub(start).Hours()
来源：http://anf.andypj.xyz

Ruby: end - start                 # 返回秒数
来源：http://dde.hnqzz.top

C#:   (end - start).TotalSeconds
来源：http://wcg.jinghuilouyu.cn

[J07] 比较两个日期
来源：http://ndt.316326.xyz

Py:   d1 < d2;  d1 == d2
来源：http://wud.pycfn.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ydr.jinqigfzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://nss.smart0.xyz


<!-- 参考信息 -->