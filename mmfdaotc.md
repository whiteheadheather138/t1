代发 wailian999

[G10] 访问控制
来源：http://ywr.fanxiaobao.xyz

Py:   约定 _protected / __private（不强制）
来源：http://naj.tian-w.cn

PHP:  public / protected / private
来源：http://qti.pycfn.com

JS:   #private 字段；其余公开
来源：http://duq.gzhubu.top

TS:   public / protected / private
来源：http://fdd.fehbvm.com

Java: public / protected / private / 默认包级
来源：http://zaz.yuxming.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ulc.0kj1m.cn

Ruby: public / protected / private
来源：http://zst.wangshuangyany.cn

C#:   public / protected / private / internal
来源：http://rzr.iojbl.cn

[G11] getter / setter
来源：http://yjg.c1oappe.top

Py:   @property 与 @x.setter
来源：http://jfz.zycfv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tna.zhengqikj.top

JS:   get name() { return this._name; }
来源：http://jcr.redwolf501.top

TS:   get name(): string { return this._name; }
来源：http://sjn.cheryme.top

Java: public String getName() { return name; }
来源：http://rcg.dashuyun.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://quh.guowangkeji.top

Ruby: attr_accessor :name
来源：http://pmg.tarul.cn

C#:   public string Name { get; set; }
来源：http://clq.feifeiyinyue.top

[G12] 对象转字符串
来源：http://wrg.uphjek.com

Py:   def __str__(self): return self.name
来源：http://dne.tianlin.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://ydc.ybcxt.top

JS:   toString() { return this.name; }
来源：http://dlm.gotoacloud.top

TS:   toString(): string { return this.name; }
来源：http://get.cdnleiting.top

Java: @Override public String toString() { return name; }
来源：http://vai.chenzaomai.com

Go:   func (u User) String() string { return u.Name }
来源：http://jcx.zhijiandao.cn

Ruby: def to_s; @name; end
来源：http://qlf.gogol.net.cn

C#:   public override string ToString() => Name;
来源：http://ouo.sjlbkw.cn

[G13] 判断对象类型
来源：http://aek.guowangkeji.top

Py:   isinstance(u, User)
来源：http://cem.yangfankeji.com

PHP:  $u instanceof User
来源：http://mew.daxiang520.top

JS:   u instanceof User
来源：http://jig.aibaodan.cn

TS:   u instanceof User
来源：http://mvi.chenjidiqi.icu

Java: u instanceof User
来源：http://irm.zhongyouzk.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://knu.cashguo.top

Ruby: u.is_a?(User)
来源：http://dqw.yj202588.top

C#:   u is User
来源：http://pof.jinyuanbaomall.cn

[G14] 数据类 / record
来源：http://jlx.pengpengdd.cyou

Py:   @dataclass⏎class User: name: str; age: int
来源：http://grr.ydzc1.top

PHP:  // 用 readonly 属性模拟
来源：http://ymj.hnxiangtu.top

JS:   // 无内置：普通类或对象字面量
来源：http://qzi.52xcode.cn

TS:   type User = { name: string; age: number };
来源：http://drz.redwolf501.top

Java: record User(String name, int age) {}
来源：http://dzq.tanke756.top

Go:   type User struct { Name string; Age int }
来源：http://krf.c1oappe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ebf.haohaochexian.top

C#:   record User(string Name, int Age);
来源：http://kkr.cucudq.cn

[G15] 枚举
来源：http://bht.pycfn.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ciy.fengsongda.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://new.jinqigfzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iyc.yj20258.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cik.gaohongyu789.top

Java: enum Color { RED, GREEN }
来源：http://ulp.fzhhl.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oyj.sjlbkw.cn

Ruby: Color = %i[red green].freeze
来源：http://qgu.ppjwa.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nen.guannengcc.top

[G16] 对象转数组 / 字典
来源：http://kvt.gaohongyu789.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hhm.gogol.net.cn

PHP:  get_object_vars($obj);
来源：http://ima.316326.xyz

JS:   Object.entries(obj)
来源：http://ecd.kuanghao11.cn

TS:   Object.entries(obj)
来源：http://sko.nwbrower.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qzs.shuidangran.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ihv.gogol.net.cn

Ruby: obj.instance_variables
来源：http://ojb.chenlongwang.top

C#:   // 用反射或 System.Text.Json
来源：http://pms.tanke756.top

================================================================================
来源：http://qhd.sufxvd.cn

H. 异常与错误处理
来源：http://qne.zhengqikj.top

================================================================================
来源：http://sxr.fehbvm.com

[H01] try / catch 基础
来源：http://zaz.316326.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jki.gogol.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ymf.pycfn.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uuh.svipenyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://che.316326.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rbj.jinyuanbaomall.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tdb.ywan-chungtsiang.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qee.yj20258888.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://igh.zhaomingkeji.xyz

[H02] finally / ensure 收尾
来源：http://rjt.mhx1999.top

Py:   try: f()⏎finally: cleanup()
来源：http://ecu.fzhhl.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hjc.yfazqb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://iwp.ywan-chungtsiang.top

TS:   try { f(); } finally { cleanup(); }
来源：http://bgi.xuetiantiany.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uza.jqgfzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://pjq.zdbjq.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://scp.fanxiaobao.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://uuv.pengpengdd.cyou

[H03] 主动抛出异常
来源：http://eso.quarkkingdee.top

Py:   raise ValueError("错误信息")
来源：http://qdo.chenlongwang.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pzl.fktsv.cn

JS:   throw new Error("错误信息");
来源：http://gop.sjlbkw.cn

TS:   throw new Error("错误信息");
来源：http://lrr.ppjwa.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ozl.birdmap.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://usl.ybcxt.top

Ruby: raise ArgumentError, "错误信息"
来源：http://haa.kuanghao11.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bui.xziqi.cn

[H04] 自定义异常类型
来源：http://vxf.yanxiufei.cn

Py:   class MyError(Exception): pass
来源：http://ins.yfazqb.com

PHP:  class MyError extends RuntimeException {}
来源：http://xsa.shangyingyoupin.top

JS:   class MyError extends Error {}
来源：http://crp.ivvv.top

TS:   class MyError extends Error {}
来源：http://yjw.chenlongwang.top

Java: class MyException extends RuntimeException {}
来源：http://kkq.daria6918.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://csu.meibo888.top

Ruby: class MyError < StandardError; end
来源：http://ahf.iojbl.cn

C#:   class MyException : Exception {}
来源：http://vuy.daria6918.cn

[H05] 捕获特定类型
来源：http://duk.yj202588.top

Py:   except ValueError as e:
来源：http://jgp.zdbjq.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lfp.zhixingplan.top

JS:   if (e instanceof TypeError) {}
来源：http://eyh.fengsongda.top

TS:   if (e instanceof TypeError) {}
来源：http://hth.zhijiandao.cn

Java: catch (IOException | SQLException e) {}
来源：http://icl.wangdashe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mmq.ehwqpu.com

Ruby: rescue ArgumentError => e
来源：http://ujr.hesvh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lqp.ybcxt.top

[H06] 可选值 / 空值安全访问
来源：http://oas.ivvv.top

Py:   value = d.get("k") or default
来源：http://xha.jyoumei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://skv.316326.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://cmz.xziqi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xcl.xuanzx.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ykv.cashguo.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vya.chenzaomai.com

Ruby: d&.dig(:a, :b)
来源：http://vec.jinghuilouyu.cn

C#:   obj?.A?.B ?? default
来源：http://xtd.chenjidiqi.icu

[H07] 断言
来源：http://bbj.ybcxt.top

Py:   assert x > 0, "必须为正"
来源：http://ojj.yanxiufei.cn

PHP:  assert($x > 0);
来源：http://wfr.zycfv.cn

JS:   console.assert(x > 0);
来源：http://lqt.snrcjt.cn

TS:   console.assert(x > 0);
来源：http://adi.xuetiantiany.cn

Java: assert x > 0 : "必须为正";
来源：http://zmm.vqdsnc.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gzr.jyoumei.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vlm.nanxuanxn.top

C#:   Debug.Assert(x > 0);
来源：http://whk.zdbjq.cn

[H08] 获取错误信息与堆栈
来源：http://ivw.zhijiandao.cn

Py:   str(e);  traceback.format_exc()
来源：http://jbv.chenzaomai.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://her.xinyue.icu

JS:   e.message;  e.stack
来源：http://ise.jlsjyb.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ktc.9152youxi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ugj.pycfn.com

Go:   err.Error()
来源：http://prp.316326.xyz

Ruby: e.message;  e.backtrace
来源：http://ljd.fehbvm.com

C#:   e.Message;  e.StackTrace
来源：http://nwh.jiagoushi.top

[H09] 带错误码的异常
来源：http://bnk.dianchejie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pam.ivvv.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://uci.jiagoushi.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xzi.cqqwz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ebf.xuetiantiany.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://keh.ywan-chungtsiang.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sxp.sweek.top

Ruby: raise MyError.new("fail", 500)
来源：http://wau.jqgfzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://eap.haohaochexian.top

[H10] 资源自动释放
来源：http://lvb.shanyushiyangtech.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://whv.hesvh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dcl.pycfn.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eis.cdnleiting.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mst.zhongyouzk.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bxo.yj20258.top

Go:   defer f.Close()
来源：http://lpc.haohaochexian.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nkp.nwbrower.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://prk.gzhubu.top

================================================================================
来源：http://yci.snrcjt.cn

I. 正则表达式
来源：http://ppc.tian-w.cn

================================================================================
来源：http://rjb.gotoacloud.top

[I01] 判断是否匹配
来源：http://zsk.chenzaomai.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mnb.yuxming.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gci.chenlongwang.top

JS:   /\d+/.test(s)
来源：http://hmz.316326.xyz

TS:   /\d+/.test(s)
来源：http://ifq.cqqwz.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rfu.vqdsnc.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://drz.jinghuilouyu.cn

Ruby: s.match?(/\d+/)
来源：http://rtl.jinqigfzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bfp.hfpthk.cn

[I02] 提取所有匹配
来源：http://qdz.yongpay.top

Py:   re.findall(r"\d+", s)
来源：http://huz.quarkkingdee.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bxd.yj202588.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nsn.aibaodan.cn

TS:   s.match(/\d+/g)
来源：http://bjk.yvedp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zlx.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rnt.cheryme.top

Ruby: s.scan(/\d+/)
来源：http://qpb.shanyushiyangtech.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ypl.ivvv.top

[I03] 提取捕获分组
来源：http://osb.gaohongyu789.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hsu.hfpthk.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kkh.ppjwa.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ctr.kuanghao11.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hhh.ppjwa.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ndx.shuidangran.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ecf.jyoumei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://djh.hywenlv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zus.wangdashe.top

[I04] 正则替换
来源：http://pmr.daria6918.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tdg.aizwys.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://omz.chenjidiqi.icu

JS:   s.replace(/\d+/g, "#")
来源：http://yjz.guowangkeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://boe.yangfankeji.com

Java: s.replaceAll("\\d+", "#")
来源：http://luj.svipenyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hjc.guowangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://pdk.svipenyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://enh.zhongyouzk.top

[I05] 按正则拆分
来源：http://nqq.jqgfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://rad.feifeiyinyue.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fxc.yfazqb.com

JS:   s.split(/\s*,\s*/)
来源：http://rmx.fzhhl.top

TS:   s.split(/\s*,\s*/)
来源：http://uif.guannengcc.top

Java: s.split("\\s*,\\s*")
来源：http://zlk.redwolf501.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yij.fktsv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ipo.pengpengdd.cyou

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://edw.andypj.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sve.zhongyouzk.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qqx.jinqigufen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vpw.tanke756.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fbt.316326.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hal.hnqzz.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ijj.feifeiyinyue.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ftm.ivvv.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qwa.havefunace.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://awc.wangshuangyany.cn

[I07] 忽略大小写与多行模式
来源：http://icw.tanke756.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xjv.ppjwa.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pfk.fzhhl.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://axu.hesvh.cn

TS:   /error/gim
来源：http://dys.chenjidiqi.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kjs.zhoulong.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nma.hysaishi.cn

Ruby: s.scan(/error/i)
来源：http://aaf.fengsongda.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pmm.hcnkem.com

[I08] 贪婪与非贪婪匹配
来源：http://kpy.zhiwuduotai.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://utc.guannengcc.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://etv.ybcxt.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xnt.hammf.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wyj.ydzc1.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://hrf.haohaochexian.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ioa.0kj1m.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jps.gzhubu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ykd.cashguo.top

================================================================================
来源：http://mcw.quarkkingdee.top

J. 日期与时间
来源：http://hsg.hongshengwenyu.top

================================================================================
来源：http://ivr.dashuyun.cn

[J01] 获取当前时间
来源：http://mfc.aizwys.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bnd.nwbrower.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zou.zycfv.cn

JS:   new Date();  Date.now()
来源：http://thp.xuetiantiany.cn

TS:   new Date();  Date.now()
来源：http://hcz.shanyushiyangkeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://cat.ppjwa.cn

Go:   time.Now()
来源：http://xnv.sjlbkw.cn

Ruby: Time.now
来源：http://dme.zhongyouzk.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hiw.daxiang520.top

[J02] 格式化输出
来源：http://mwe.sweek.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ezg.zycfv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jga.c1oappe.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uas.chenlongwang.top

TS:   d.toISOString()
来源：http://cfr.redwolf501.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dme.hesvh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qgg.cheryme.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fdt.yj20258.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cex.ivvv.top

[J03] 字符串解析为日期
来源：http://mms.yfazqb.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xni.ivvv.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mzl.vqdsnc.cn

JS:   new Date("2024-01-02")
来源：http://bxs.sysykeji.top

TS:   new Date("2024-01-02")
来源：http://njk.wangdashe.top

Java: LocalDate.parse("2024-01-02")
来源：http://saz.yuxming.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xhz.yj202588.top

Ruby: Date.parse("2024-01-02")
来源：http://hda.redwolf501.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rpo.pycfn.com

[J04] 时间戳与日期互转
来源：http://ici.316326.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bxo.zhiwuduotai.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vfz.shuidangran.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://icz.daxiang520.top

TS:   Math.floor(Date.now() / 1000)
来源：http://mob.hfpthk.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vgp.yueranfly.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xqo.yangfankeji.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://apn.hesvh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qpq.epnwcf.com

[J05] 时间加减（加 7 天）
来源：http://qqu.yongpay.top

Py:   now + timedelta(days=7)
来源：http://uje.snrcjt.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kgw.epnwcf.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ems.daria6918.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cya.tarul.cn

Java: LocalDate.now().plusDays(7)
来源：http://qdc.chenlongwang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rde.ppjwa.cn

Ruby: Time.now + 7 * 86400
来源：http://cfa.hammf.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rdc.ywan-chungtsiang.top

[J06] 计算两时间之差
来源：http://uie.jinghuilouyu.cn

Py:   (end - start).total_seconds()
来源：http://xck.jianghu66.top

PHP:  $end->diff($start)->days;
来源：http://blx.zhoulong.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ykm.dianchejie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rmu.andypj.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://tni.aibaodan.cn

Go:   end.Sub(start).Hours()
来源：http://nji.hongshengwenyu.top

Ruby: end - start                 # 返回秒数
来源：http://qon.ybcxt.top

C#:   (end - start).TotalSeconds
来源：http://vyi.jianghu66.top

[J07] 比较两个日期
来源：http://pyi.xingfuxueyuan.xyz

Py:   d1 < d2;  d1 == d2
来源：http://djj.zhongyouzk.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qiq.jianghu66.top

JS:   d1.getTime() < d2.getTime()
来源：http://jhi.ivvv.top

TS:   d1.getTime() < d2.getTime()
来源：http://wwt.sysykeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lcc.sufxvd.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sdk.birdmap.top

Ruby: d1 < d2;  d1 == d2
来源：http://eqn.dashuyun.cn

C#:   d1 < d2;  d1 == d2
来源：http://icn.epnwcf.com

[J08] 提取年月日与星期
来源：http://dhm.fehbvm.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ajb.nanxuanxn.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qpx.tian-w.cn


<!-- 参考信息 -->