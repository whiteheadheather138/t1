代发 wailian999

Java: interface Shape { double area(); }
来源：http://pij.tianlin.xyz

Go:   type Shape interface { Area() float64 }
来源：http://qjy.9152youxi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wgn.tian-w.cn

C#:   interface IShape { double Area(); }
来源：http://cnu.xziqi.cn

[G10] 访问控制
来源：http://zxh.shzxlz.cn

Py:   约定 _protected / __private（不强制）
来源：http://gij.zhiwuduotai.top

PHP:  public / protected / private
来源：http://hmu.chenjidiqi.icu

JS:   #private 字段；其余公开
来源：http://dxq.nanxinkj.top

TS:   public / protected / private
来源：http://oir.xuetiantiany.cn

Java: public / protected / private / 默认包级
来源：http://xqp.zdqjudy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://chv.zycfv.cn

Ruby: public / protected / private
来源：http://wow.ydjk.org.cn

C#:   public / protected / private / internal
来源：http://osb.fehbvm.com

[G11] getter / setter
来源：http://gqu.snrcjt.cn

Py:   @property 与 @x.setter
来源：http://jpx.vehdjk.com

PHP:  public function getName(): string { return $this->name; }
来源：http://cxc.zycfv.cn

JS:   get name() { return this._name; }
来源：http://ela.xuetiantiany.cn

TS:   get name(): string { return this._name; }
来源：http://emt.zhongyouzk.top

Java: public String getName() { return name; }
来源：http://pap.yj202588.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://miq.zhoulong.xyz

Ruby: attr_accessor :name
来源：http://lpf.zhaomingkeji.xyz

C#:   public string Name { get; set; }
来源：http://bml.ydzc1.top

[G12] 对象转字符串
来源：http://ocx.nanxinkj.top

Py:   def __str__(self): return self.name
来源：http://lsy.316326.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://qib.jinqigfzy.top

JS:   toString() { return this.name; }
来源：http://hej.zdbjq.cn

TS:   toString(): string { return this.name; }
来源：http://bgw.daxiang520.top

Java: @Override public String toString() { return name; }
来源：http://qij.yj20258.top

Go:   func (u User) String() string { return u.Name }
来源：http://bxq.fktsv.cn

Ruby: def to_s; @name; end
来源：http://rnt.xylfe.cn

C#:   public override string ToString() => Name;
来源：http://ail.birdmap.top

[G13] 判断对象类型
来源：http://mzn.hnqzz.top

Py:   isinstance(u, User)
来源：http://ixj.pengpengdd.cyou

PHP:  $u instanceof User
来源：http://sxr.meibo888.top

JS:   u instanceof User
来源：http://mmm.ctjpmb.com

TS:   u instanceof User
来源：http://dct.zhixingplan.top

Java: u instanceof User
来源：http://wke.chenjidiqi.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://wzl.ppjwa.cn

Ruby: u.is_a?(User)
来源：http://shm.hnxiangtu.top

C#:   u is User
来源：http://ggo.yuanzhike.top

[G14] 数据类 / record
来源：http://pih.haohaochexian.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kca.xingfuxueyuan.xyz

PHP:  // 用 readonly 属性模拟
来源：http://nzz.svipenyu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://igl.bjfxy.top

TS:   type User = { name: string; age: number };
来源：http://ymq.cqqwz.cn

Java: record User(String name, int age) {}
来源：http://vzl.gotoacloud.top

Go:   type User struct { Name string; Age int }
来源：http://vqk.zhongyouzk.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dzs.uphjek.com

C#:   record User(string Name, int Age);
来源：http://yxx.nanxinkj.top

[G15] 枚举
来源：http://zzm.vqdsnc.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bro.shzxlz.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://iua.nanxuanxn.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ixo.nanxinkj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dwb.nanxuanxn.top

Java: enum Color { RED, GREEN }
来源：http://slv.jlsjyb.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qbm.gaohongyu789.top

Ruby: Color = %i[red green].freeze
来源：http://csx.xinyue.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tst.tanke756.top

[G16] 对象转数组 / 字典
来源：http://ydx.jinqigufen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://iho.hnqzz.top

PHP:  get_object_vars($obj);
来源：http://bfc.gaohongyu789.top

JS:   Object.entries(obj)
来源：http://vuu.xuetiantiany.cn

TS:   Object.entries(obj)
来源：http://elb.nwbrower.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jvp.hywenlv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kkd.bjfxy.top

Ruby: obj.instance_variables
来源：http://rvs.snrcjt.cn

C#:   // 用反射或 System.Text.Json
来源：http://fft.fanxiaobao.xyz

================================================================================
来源：http://bhs.ivvv.top

H. 异常与错误处理
来源：http://rie.ywan-chungtsiang.top

================================================================================
来源：http://qji.quarkkingdee.top

[H01] try / catch 基础
来源：http://qwt.xziqi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pvq.chenjidiqi.icu

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nep.snrcjt.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bcf.gogol.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fko.ppjwa.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jmw.uphjek.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://emv.jqgufenzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wjo.gzhubu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ywk.cucudq.cn

[H02] finally / ensure 收尾
来源：http://npx.xingfuxueyuan.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://isz.vehdjk.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://nwe.316326.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://gda.andypj.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://wml.nwbrower.top

Java: try { f(); } finally { cleanup(); }
来源：http://phm.daxiang520.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://efz.ctjpmb.com

Ruby: begin; f; ensure; cleanup; end
来源：http://pec.andypj.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://pfa.shzxlz.cn

[H03] 主动抛出异常
来源：http://aya.tian-w.cn

Py:   raise ValueError("错误信息")
来源：http://psq.c1oappe.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ooh.ybcxt.top

JS:   throw new Error("错误信息");
来源：http://ftb.tian-w.cn

TS:   throw new Error("错误信息");
来源：http://kvz.yueranfly.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hpl.fktsv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ghi.fengsongda.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jpv.fzhhl.top

C#:   throw new ArgumentException("错误信息");
来源：http://vnc.aizwys.cn

[H04] 自定义异常类型
来源：http://zzl.fzhhl.top

Py:   class MyError(Exception): pass
来源：http://kut.jyoumei.cn

PHP:  class MyError extends RuntimeException {}
来源：http://egf.fehbvm.com

JS:   class MyError extends Error {}
来源：http://pzq.uphjek.com

TS:   class MyError extends Error {}
来源：http://ytc.daxiang520.top

Java: class MyException extends RuntimeException {}
来源：http://kze.ppjwa.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ldy.yj20258888.top

Ruby: class MyError < StandardError; end
来源：http://ucz.andypj.xyz

C#:   class MyException : Exception {}
来源：http://uoz.aizwys.cn

[H05] 捕获特定类型
来源：http://nma.nwbrower.top

Py:   except ValueError as e:
来源：http://saa.316326.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wyl.jqgfzy.top

JS:   if (e instanceof TypeError) {}
来源：http://owb.zycfv.cn

TS:   if (e instanceof TypeError) {}
来源：http://eyd.hongshengwenyu.top

Java: catch (IOException | SQLException e) {}
来源：http://aea.zhengqikj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qvi.daria6918.cn

Ruby: rescue ArgumentError => e
来源：http://gud.fanxiaobao.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tpj.ydzc1.top

[H06] 可选值 / 空值安全访问
来源：http://cxo.316326.xyz

Py:   value = d.get("k") or default
来源：http://tsv.ppjwa.cn

PHP:  $v = $d["k"] ?? null;
来源：http://raj.shanyushiyangkeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://dmv.fanxiaobao.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://hzc.redwolf501.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://aiv.yuxming.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ilu.hnqzz.top

Ruby: d&.dig(:a, :b)
来源：http://xeq.tianlin.xyz

C#:   obj?.A?.B ?? default
来源：http://rar.xuanzx.com

[H07] 断言
来源：http://usg.xuetiantiany.cn

Py:   assert x > 0, "必须为正"
来源：http://ebg.jinyuanbaomall.cn

PHP:  assert($x > 0);
来源：http://qjr.zhixingplan.top

JS:   console.assert(x > 0);
来源：http://wdp.tarul.cn

TS:   console.assert(x > 0);
来源：http://mvo.sjlbkw.cn

Java: assert x > 0 : "必须为正";
来源：http://zjm.cqqwz.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ilq.sufxvd.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ygx.shanyushiyangkeji.top

C#:   Debug.Assert(x > 0);
来源：http://apj.sxryk.cn

[H08] 获取错误信息与堆栈
来源：http://tiy.hywenlv.cn

Py:   str(e);  traceback.format_exc()
来源：http://jqs.chenjidiqi.icu

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nwg.yanxiufei.cn

JS:   e.message;  e.stack
来源：http://koa.fehbvm.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://tys.shanyushiyangtech.top

Java: e.getMessage();  e.printStackTrace()
来源：http://nae.guowangkeji.top

Go:   err.Error()
来源：http://ekk.aizwys.cn

Ruby: e.message;  e.backtrace
来源：http://fkp.jyoumei.cn

C#:   e.Message;  e.StackTrace
来源：http://mjz.ehwqpu.com

[H09] 带错误码的异常
来源：http://szw.zhengqikj.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ksy.fktsv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cpv.fengsongda.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pfu.ehwqpu.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ucg.tarul.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jdw.zhongyouzk.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rht.svipenyu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://olm.sufxvd.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ekt.pycfn.com

[H10] 资源自动释放
来源：http://bcg.snrcjt.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://igx.vehdjk.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://emq.jiagoushi.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jqq.zdqjudy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zhw.guowangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tjm.meibo888.top

Go:   defer f.Close()
来源：http://joa.tanke756.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yin.shangyingyoupin.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kfp.aibaodan.cn

================================================================================
来源：http://ary.316326.xyz

I. 正则表达式
来源：http://lyj.ehwqpu.com

================================================================================
来源：http://qsz.nanxuanxn.top

[I01] 判断是否匹配
来源：http://duw.feifeiyinyue.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xlz.0kj1m.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tff.gzhubu.top

JS:   /\d+/.test(s)
来源：http://nnt.zhoulong.xyz

TS:   /\d+/.test(s)
来源：http://flp.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sqy.sjlbkw.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://buv.andypj.xyz

Ruby: s.match?(/\d+/)
来源：http://pao.hywenlv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://upg.hnqzz.top

[I02] 提取所有匹配
来源：http://xsq.zhoulong.xyz

Py:   re.findall(r"\d+", s)
来源：http://dqq.jqgufenzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://egu.jiagoushi.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://iff.9152youxi.cn

TS:   s.match(/\d+/g)
来源：http://dal.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zle.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xbr.zhiwuduotai.top

Ruby: s.scan(/\d+/)
来源：http://ofj.cucudq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uza.0kj1m.cn

[I03] 提取捕获分组
来源：http://ndh.c1oappe.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://akg.smart0.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://iuv.kuanghao11.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wml.nwbrower.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rtn.dianchejie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wdj.mhx1999.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://poi.cqqwz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sji.snrcjt.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://prj.xinyue.icu

[I04] 正则替换
来源：http://reb.sufxvd.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://elm.jlsjyb.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cwm.c1oappe.top

JS:   s.replace(/\d+/g, "#")
来源：http://fei.redwolf501.top

TS:   s.replace(/\d+/g, "#")
来源：http://bkt.snrcjt.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jnd.fehbvm.com

Go:   re.ReplaceAllString(s, "#")
来源：http://eyt.nanxinkj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://yma.smart0.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xco.sweek.top

[I05] 按正则拆分
来源：http://rib.guannengcc.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ron.ehwqpu.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cpq.cucudq.cn

JS:   s.split(/\s*,\s*/)
来源：http://ksm.c1oappe.top

TS:   s.split(/\s*,\s*/)
来源：http://dhy.pycfn.com

Java: s.split("\\s*,\\s*")
来源：http://agg.yj20258.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://akc.jqgfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://ces.mhx1999.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aln.0kj1m.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cyh.ybcxt.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uio.hysaishi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vin.9152youxi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pcf.jianghu66.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yas.hesvh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hmz.ctjpmb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fim.hfpthk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://abh.redwolf501.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://piv.ehwqpu.com

[I07] 忽略大小写与多行模式
来源：http://fwb.shanyushiyangtech.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zsm.hnxiangtu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qkp.yfazqb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rco.nanxinkj.top

TS:   /error/gim
来源：http://axr.chenlongwang.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nxc.quarkkingdee.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kdi.sysykeji.top

Ruby: s.scan(/error/i)
来源：http://wqj.yongpay.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://amk.ydjk.org.cn

[I08] 贪婪与非贪婪匹配
来源：http://rny.dianchejie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nbi.hnxiangtu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://faw.wangdashe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zbv.jinyuanbaomall.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://iyp.jinghuilouyu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jfk.hysaishi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sdc.fzhhl.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kjf.nanxuanxn.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lge.pycfn.com

================================================================================
来源：http://jik.quarkkingdee.top

J. 日期与时间
来源：http://jam.hywenlv.cn

================================================================================
来源：http://opw.ppjwa.cn

[J01] 获取当前时间
来源：http://ten.gotoacloud.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://yze.nanxinkj.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yiv.cdnleiting.top

JS:   new Date();  Date.now()
来源：http://jcg.guannengcc.top

TS:   new Date();  Date.now()
来源：http://ldq.daxiang520.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dkf.nwbrower.top

Go:   time.Now()
来源：http://orn.tian-w.cn

Ruby: Time.now
来源：http://gpa.fanxiaobao.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dqt.52xcode.cn

[J02] 格式化输出
来源：http://bgf.ehwqpu.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kvq.0kj1m.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://euq.zhiwuduotai.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oeb.aibaodan.cn

TS:   d.toISOString()
来源：http://itj.jiagoushi.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://urh.zdqjudy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vdf.0kj1m.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dxj.tanke756.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zev.yangfankeji.com

[J03] 字符串解析为日期
来源：http://qfg.jlsjyb.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hxp.cdnleiting.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pmq.yongpay.top

JS:   new Date("2024-01-02")
来源：http://cwy.jinyuanbaomall.cn

TS:   new Date("2024-01-02")
来源：http://ctf.vehdjk.com

Java: LocalDate.parse("2024-01-02")
来源：http://qyq.c1oappe.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://flm.ydzc1.top

Ruby: Date.parse("2024-01-02")
来源：http://mle.gaohongyu789.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hay.jqgfzy.top

[J04] 时间戳与日期互转
来源：http://ewi.xylfe.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jys.zhiwuduotai.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://htb.jianghu66.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://afu.xingfuxueyuan.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://nhz.yonumen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://snb.ehwqpu.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://juq.daxiang520.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cus.wangshuangyany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sni.yuanzhike.top

[J05] 时间加减（加 7 天）
来源：http://fha.zhaomingkeji.xyz

Py:   now + timedelta(days=7)
来源：http://nwa.xuanzx.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://hmj.vehdjk.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vky.hysaishi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pti.ivvv.top

Java: LocalDate.now().plusDays(7)
来源：http://ead.52xcode.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jqj.chenjidiqi.icu

Ruby: Time.now + 7 * 86400
来源：http://eie.ehwqpu.com

C#:   DateTime.Now.AddDays(7)
来源：http://lko.tanke756.top

[J06] 计算两时间之差
来源：http://lxv.yuxming.cn

Py:   (end - start).total_seconds()
来源：http://dew.yueranfly.top

PHP:  $end->diff($start)->days;
来源：http://lrc.52xcode.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ojd.quarkkingdee.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eeq.xylfe.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jgu.yanxiufei.cn

Go:   end.Sub(start).Hours()
来源：http://hbz.havefunace.top

Ruby: end - start                 # 返回秒数
来源：http://rci.yangfankeji.com

C#:   (end - start).TotalSeconds
来源：http://xog.vehdjk.com

[J07] 比较两个日期
来源：http://kcj.52xcode.cn

Py:   d1 < d2;  d1 == d2
来源：http://nvj.xuanzx.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rzq.ctjpmb.com

JS:   d1.getTime() < d2.getTime()
来源：http://ale.yj202588.top

TS:   d1.getTime() < d2.getTime()
来源：http://bmy.jiagoushi.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://olu.uphjek.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qko.gogol.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://deu.9152youxi.cn


<!-- 参考信息 -->