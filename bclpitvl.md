代发 wailian999

[G10] 访问控制
来源：http://bfa.dashuyun.cn

Py:   约定 _protected / __private（不强制）
来源：http://lsk.ybcxt.top

PHP:  public / protected / private
来源：http://djy.jqgufenzy.top

JS:   #private 字段；其余公开
来源：http://mvw.sysykeji.top

TS:   public / protected / private
来源：http://xjd.hysaishi.cn

Java: public / protected / private / 默认包级
来源：http://gjk.zhongyouzk.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://pkd.yuanzhike.top

Ruby: public / protected / private
来源：http://njw.snrcjt.cn

C#:   public / protected / private / internal
来源：http://oee.uphjek.com

[G11] getter / setter
来源：http://chi.jlsjyb.cn

Py:   @property 与 @x.setter
来源：http://xsd.vehdjk.com

PHP:  public function getName(): string { return $this->name; }
来源：http://ndn.sweek.top

JS:   get name() { return this._name; }
来源：http://wlh.jiagoushi.top

TS:   get name(): string { return this._name; }
来源：http://lns.snrcjt.cn

Java: public String getName() { return name; }
来源：http://pli.fzhhl.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ovh.smart0.xyz

Ruby: attr_accessor :name
来源：http://jrm.gaohongyu789.top

C#:   public string Name { get; set; }
来源：http://mft.kuanghao11.cn

[G12] 对象转字符串
来源：http://inj.daxiang520.top

Py:   def __str__(self): return self.name
来源：http://tek.feifeiyinyue.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://gtk.cucudq.cn

JS:   toString() { return this.name; }
来源：http://zwx.ybcxt.top

TS:   toString(): string { return this.name; }
来源：http://qtg.shzxlz.cn

Java: @Override public String toString() { return name; }
来源：http://fbf.nanxinkj.top

Go:   func (u User) String() string { return u.Name }
来源：http://guj.xuetiantiany.cn

Ruby: def to_s; @name; end
来源：http://pyr.jinghuilouyu.cn

C#:   public override string ToString() => Name;
来源：http://qpw.xuanzx.com

[G13] 判断对象类型
来源：http://fho.zhiwuduotai.top

Py:   isinstance(u, User)
来源：http://tfq.hnqzz.top

PHP:  $u instanceof User
来源：http://gyn.meibo888.top

JS:   u instanceof User
来源：http://epw.yfazqb.com

TS:   u instanceof User
来源：http://mce.ywan-chungtsiang.top

Java: u instanceof User
来源：http://mgi.tianlin.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://awz.sxryk.cn

Ruby: u.is_a?(User)
来源：http://nys.jinghuilouyu.cn

C#:   u is User
来源：http://cky.ivvv.top

[G14] 数据类 / record
来源：http://tkr.cucudq.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sej.316326.xyz

PHP:  // 用 readonly 属性模拟
来源：http://ave.gzhubu.top

JS:   // 无内置：普通类或对象字面量
来源：http://uyi.jianghu66.top

TS:   type User = { name: string; age: number };
来源：http://gmp.aibaodan.cn

Java: record User(String name, int age) {}
来源：http://vxe.vehdjk.com

Go:   type User struct { Name string; Age int }
来源：http://kyt.316326.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ptx.hongshengwenyu.top

C#:   record User(string Name, int Age);
来源：http://fdt.meibo888.top

[G15] 枚举
来源：http://bdq.guannengcc.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vqr.bjfxy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://miq.chenjidiqi.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zef.hnxiangtu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jsy.0kj1m.cn

Java: enum Color { RED, GREEN }
来源：http://uxs.xuanzx.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cxg.zdqjudy.top

Ruby: Color = %i[red green].freeze
来源：http://byr.gaohongyu789.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pmo.ywan-chungtsiang.top

[G16] 对象转数组 / 字典
来源：http://nqu.cucudq.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ulh.yonumen.top

PHP:  get_object_vars($obj);
来源：http://vlu.ydzc1.top

JS:   Object.entries(obj)
来源：http://rih.hysaishi.cn

TS:   Object.entries(obj)
来源：http://hmo.jqgufenzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blc.hammf.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xgb.fanxiaobao.xyz

Ruby: obj.instance_variables
来源：http://hzq.sjlbkw.cn

C#:   // 用反射或 System.Text.Json
来源：http://tbq.c1oappe.top

================================================================================
来源：http://rzr.hysaishi.cn

H. 异常与错误处理
来源：http://yqo.52xcode.cn

================================================================================
来源：http://oft.mhx1999.top

[H01] try / catch 基础
来源：http://wuq.feifeiyinyue.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kci.yvedp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hzp.chenzaomai.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://aut.quarkkingdee.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jfa.zdbjq.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dcl.hnxiangtu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dec.sufxvd.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yeq.ivvv.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zrx.nanxinkj.top

[H02] finally / ensure 收尾
来源：http://zut.yuxming.cn

Py:   try: f()⏎finally: cleanup()
来源：http://iop.nanxinkj.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://axk.xingfuxueyuan.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://mlc.hcnkem.com

TS:   try { f(); } finally { cleanup(); }
来源：http://xta.yfazqb.com

Java: try { f(); } finally { cleanup(); }
来源：http://ryl.guannengcc.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://pdh.ydzc1.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kfa.hcnkem.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://kcf.sweek.top

[H03] 主动抛出异常
来源：http://eqd.yvedp.cn

Py:   raise ValueError("错误信息")
来源：http://dgu.redwolf501.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wfr.hcnkem.com

JS:   throw new Error("错误信息");
来源：http://jvr.sufxvd.cn

TS:   throw new Error("错误信息");
来源：http://nhl.hammf.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hap.kuanghao11.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sls.jinqigfzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ual.yj20258888.top

C#:   throw new ArgumentException("错误信息");
来源：http://bvs.hnqzz.top

[H04] 自定义异常类型
来源：http://hhi.sjlbkw.cn

Py:   class MyError(Exception): pass
来源：http://fxr.vehdjk.com

PHP:  class MyError extends RuntimeException {}
来源：http://cpl.mhx1999.top

JS:   class MyError extends Error {}
来源：http://nuj.jqgfzy.top

TS:   class MyError extends Error {}
来源：http://qjr.9152youxi.cn

Java: class MyException extends RuntimeException {}
来源：http://idl.chenzaomai.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pha.yuanzhike.top

Ruby: class MyError < StandardError; end
来源：http://nqu.9152youxi.cn

C#:   class MyException : Exception {}
来源：http://gop.redwolf501.top

[H05] 捕获特定类型
来源：http://xml.zhijiandao.cn

Py:   except ValueError as e:
来源：http://zsm.mhx1999.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pcj.cdnleiting.top

JS:   if (e instanceof TypeError) {}
来源：http://mtj.jinyuanbaomall.cn

TS:   if (e instanceof TypeError) {}
来源：http://isb.c1oappe.top

Java: catch (IOException | SQLException e) {}
来源：http://ajg.mhx1999.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://osx.fengsongda.top

Ruby: rescue ArgumentError => e
来源：http://yei.tianlin.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pvd.ehwqpu.com

[H06] 可选值 / 空值安全访问
来源：http://osj.chenjidiqi.icu

Py:   value = d.get("k") or default
来源：http://zhk.chenzaomai.com

PHP:  $v = $d["k"] ?? null;
来源：http://ihe.shzxlz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mlg.hfpthk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wkq.c1oappe.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mmm.9152youxi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bax.fengsongda.top

Ruby: d&.dig(:a, :b)
来源：http://myq.ctjpmb.com

C#:   obj?.A?.B ?? default
来源：http://mat.zhixingplan.top

[H07] 断言
来源：http://tqo.fzhhl.top

Py:   assert x > 0, "必须为正"
来源：http://eaz.ppjwa.cn

PHP:  assert($x > 0);
来源：http://iqj.zhoulong.xyz

JS:   console.assert(x > 0);
来源：http://zby.dianchejie.cn

TS:   console.assert(x > 0);
来源：http://tjp.hesvh.cn

Java: assert x > 0 : "必须为正";
来源：http://hme.jianghu66.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bqk.iojbl.cn

Ruby: raise "必须为正" unless x > 0
来源：http://igw.epnwcf.com

C#:   Debug.Assert(x > 0);
来源：http://yrb.jqgufenzy.top

[H08] 获取错误信息与堆栈
来源：http://qvv.zhongyouzk.top

Py:   str(e);  traceback.format_exc()
来源：http://qnf.jinqigfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ocp.sxryk.cn

JS:   e.message;  e.stack
来源：http://nmq.shangyingyoupin.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://zvo.cdnleiting.top

Java: e.getMessage();  e.printStackTrace()
来源：http://yol.cdnleiting.top

Go:   err.Error()
来源：http://kzm.pycfn.com

Ruby: e.message;  e.backtrace
来源：http://mqz.tian-w.cn

C#:   e.Message;  e.StackTrace
来源：http://nhj.tarul.cn

[H09] 带错误码的异常
来源：http://tvv.xylfe.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://msa.wangshuangyany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ndq.haohaochexian.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bfw.ctjpmb.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cne.tarul.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dna.cqqwz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ray.gaohongyu789.top

Ruby: raise MyError.new("fail", 500)
来源：http://dhs.shanyushiyangtech.top

C#:   // 自定义异常类中加 Code 属性
来源：http://osa.jqgfzy.top

[H10] 资源自动释放
来源：http://wng.zhongyouzk.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://cda.daxiang520.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lpx.316326.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wug.yuxming.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ozu.ydzc1.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lnj.gzhubu.top

Go:   defer f.Close()
来源：http://wdy.yj20258888.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ooa.pengpengdd.cyou

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cqx.316326.xyz

================================================================================
来源：http://ocu.zhijiandao.cn

I. 正则表达式
来源：http://pwt.ehwqpu.com

================================================================================
来源：http://usz.cdnleiting.top

[I01] 判断是否匹配
来源：http://bgz.haohaochexian.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ygc.xuetiantiany.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jbx.pycfn.com

JS:   /\d+/.test(s)
来源：http://nqq.gaohongyu789.top

TS:   /\d+/.test(s)
来源：http://puw.jqgfzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zjr.yangfankeji.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qsx.shzxlz.cn

Ruby: s.match?(/\d+/)
来源：http://ogn.bbcook.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rxu.yfazqb.com

[I02] 提取所有匹配
来源：http://cxd.dianchejie.cn

Py:   re.findall(r"\d+", s)
来源：http://lzq.epnwcf.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vcn.dashuyun.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bdn.ppjwa.cn

TS:   s.match(/\d+/g)
来源：http://gvf.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wpc.zhixingplan.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dsb.cucudq.cn

Ruby: s.scan(/\d+/)
来源：http://trc.zhixingplan.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bhn.fktsv.cn

[I03] 提取捕获分组
来源：http://tee.chenzaomai.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tdt.tian-w.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gbf.zycfv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yrq.ywan-chungtsiang.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vmi.vehdjk.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tye.jqgfzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gzg.dianchejie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qng.sxryk.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ves.hnqzz.top

[I04] 正则替换
来源：http://bzp.nanxuanxn.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hoi.fehbvm.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wnu.xinyue.icu

JS:   s.replace(/\d+/g, "#")
来源：http://pae.daxiang520.top

TS:   s.replace(/\d+/g, "#")
来源：http://nrt.gogol.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hss.yfazqb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://gtl.fanxiaobao.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://qat.yuxming.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qyr.yongpay.top

[I05] 按正则拆分
来源：http://rno.sxryk.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dio.hfpthk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xra.haohaochexian.top

JS:   s.split(/\s*,\s*/)
来源：http://wkv.tian-w.cn

TS:   s.split(/\s*,\s*/)
来源：http://ltz.yonumen.top

Java: s.split("\\s*,\\s*")
来源：http://bxb.shuidangran.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mqh.tianlin.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://iql.shuidangran.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ici.havefunace.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kya.bjfxy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xiw.c1oappe.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jnm.hysaishi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://esm.daria6918.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uzp.shanyushiyangtech.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gvj.jinghuilouyu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kki.yj20258888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ibs.feifeiyinyue.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oqo.gzhubu.top

[I07] 忽略大小写与多行模式
来源：http://rnh.xingfuxueyuan.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rdl.zhijiandao.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fxc.chenjidiqi.icu

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gol.hcnkem.com

TS:   /error/gim
来源：http://drg.chenzaomai.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xzw.zhijiandao.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://djy.ivvv.top

Ruby: s.scan(/error/i)
来源：http://eyl.zdbjq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kix.hysaishi.cn

[I08] 贪婪与非贪婪匹配
来源：http://dnq.jianghu66.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ogi.ppjwa.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gex.daria6918.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://drz.nanxinkj.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qss.redwolf501.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wbz.daxiang520.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://okp.hcnkem.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oyn.gotoacloud.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ucg.svipenyu.cn

================================================================================
来源：http://hmf.shanyushiyangkeji.top

J. 日期与时间
来源：http://cck.cucudq.cn

================================================================================
来源：http://gvp.jinqigufen.top

[J01] 获取当前时间
来源：http://uga.jinqigufen.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ynd.zhaomingkeji.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dio.yongpay.top

JS:   new Date();  Date.now()
来源：http://ays.fehbvm.com

TS:   new Date();  Date.now()
来源：http://egi.snrcjt.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lmh.daxiang520.top

Go:   time.Now()
来源：http://dle.meibo888.top

Ruby: Time.now
来源：http://ddg.meibo888.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tjp.ydjk.org.cn

[J02] 格式化输出
来源：http://rga.shuidangran.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wvz.yonumen.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wfd.ppjwa.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bpw.ydzc1.top

TS:   d.toISOString()
来源：http://xdf.hcnkem.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gqr.yonumen.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://njn.sxryk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lfn.jlsjyb.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://awc.pycfn.com

[J03] 字符串解析为日期
来源：http://djm.0kj1m.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eyl.snrcjt.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sos.yfazqb.com

JS:   new Date("2024-01-02")
来源：http://hzw.yanxiufei.cn

TS:   new Date("2024-01-02")
来源：http://xbd.guannengcc.top

Java: LocalDate.parse("2024-01-02")
来源：http://uuc.aizwys.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hsr.yueranfly.top

Ruby: Date.parse("2024-01-02")
来源：http://udb.ctjpmb.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hwj.sweek.top

[J04] 时间戳与日期互转
来源：http://hhz.zhixingplan.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fna.wangshuangyany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dbd.kuanghao11.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fyr.jinqigufen.top

TS:   Math.floor(Date.now() / 1000)
来源：http://njz.9152youxi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sam.yfazqb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gfm.fanxiaobao.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://odw.yangfankeji.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yvh.fengsongda.top

[J05] 时间加减（加 7 天）
来源：http://agq.tianlin.xyz

Py:   now + timedelta(days=7)
来源：http://mul.zhixingplan.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://tuw.hnxiangtu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uju.9152youxi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oln.zhongyouzk.top

Java: LocalDate.now().plusDays(7)
来源：http://pcy.jinqigfzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dxq.hesvh.cn

Ruby: Time.now + 7 * 86400
来源：http://qkk.epnwcf.com

C#:   DateTime.Now.AddDays(7)
来源：http://sgk.shuidangran.top

[J06] 计算两时间之差
来源：http://vzp.tarul.cn

Py:   (end - start).total_seconds()
来源：http://euw.meibo888.top

PHP:  $end->diff($start)->days;
来源：http://xlr.fengsongda.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mmk.svipenyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hrp.hywenlv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hpc.svipenyu.cn

Go:   end.Sub(start).Hours()
来源：http://ulv.daxiang520.top

Ruby: end - start                 # 返回秒数
来源：http://wrw.cdnleiting.top

C#:   (end - start).TotalSeconds
来源：http://ekr.cucudq.cn

[J07] 比较两个日期
来源：http://nzg.jianghu66.top

Py:   d1 < d2;  d1 == d2
来源：http://izc.xingfuxueyuan.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mlw.kuanghao11.cn

JS:   d1.getTime() < d2.getTime()
来源：http://run.yonumen.top

TS:   d1.getTime() < d2.getTime()
来源：http://ted.yfazqb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ehc.dianchejie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bkg.zhijiandao.cn

Ruby: d1 < d2;  d1 == d2
来源：http://dsn.havefunace.top

C#:   d1 < d2;  d1 == d2
来源：http://acu.kuanghao11.cn

[J08] 提取年月日与星期
来源：http://rbi.daria6918.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dcw.52xcode.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ceu.fehbvm.com


<!-- 参考信息 -->