代发 wailian999

[G10] 访问控制
来源：http://dal.chenjidiqi.icu

Py:   约定 _protected / __private（不强制）
来源：http://iwm.gotoacloud.top

PHP:  public / protected / private
来源：http://fhe.svipenyu.cn

JS:   #private 字段；其余公开
来源：http://dmy.havefunace.top

TS:   public / protected / private
来源：http://xip.quarkkingdee.top

Java: public / protected / private / 默认包级
来源：http://wls.svipenyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hwk.jyoumei.cn

Ruby: public / protected / private
来源：http://hnn.pengpengdd.cyou

C#:   public / protected / private / internal
来源：http://bqo.jlsjyb.cn

[G11] getter / setter
来源：http://zvd.hammf.cn

Py:   @property 与 @x.setter
来源：http://ozj.jqgfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dlt.tarul.cn

JS:   get name() { return this._name; }
来源：http://llo.smart0.xyz

TS:   get name(): string { return this._name; }
来源：http://nrx.xylfe.cn

Java: public String getName() { return name; }
来源：http://zzl.xuetiantiany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yzc.jianghu66.top

Ruby: attr_accessor :name
来源：http://bbu.guannengcc.top

C#:   public string Name { get; set; }
来源：http://gig.zhixingplan.top

[G12] 对象转字符串
来源：http://tql.shuidangran.top

Py:   def __str__(self): return self.name
来源：http://mor.0kj1m.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fys.yuxming.cn

JS:   toString() { return this.name; }
来源：http://kqh.haohaochexian.top

TS:   toString(): string { return this.name; }
来源：http://iov.jqgufenzy.top

Java: @Override public String toString() { return name; }
来源：http://jic.hcnkem.com

Go:   func (u User) String() string { return u.Name }
来源：http://fnm.sysykeji.top

Ruby: def to_s; @name; end
来源：http://gbi.316326.xyz

C#:   public override string ToString() => Name;
来源：http://otu.nanxinkj.top

[G13] 判断对象类型
来源：http://idt.xziqi.cn

Py:   isinstance(u, User)
来源：http://xmf.kuanghao11.cn

PHP:  $u instanceof User
来源：http://zez.redwolf501.top

JS:   u instanceof User
来源：http://czx.sufxvd.cn

TS:   u instanceof User
来源：http://vnq.cashguo.top

Java: u instanceof User
来源：http://acf.jianghu66.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ilb.daxiang520.top

Ruby: u.is_a?(User)
来源：http://rlj.aibaodan.cn

C#:   u is User
来源：http://tqr.kuanghao11.cn

[G14] 数据类 / record
来源：http://hgj.andypj.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ppb.ywan-chungtsiang.top

PHP:  // 用 readonly 属性模拟
来源：http://oox.shanyushiyangkeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://mab.havefunace.top

TS:   type User = { name: string; age: number };
来源：http://mxw.nwbrower.top

Java: record User(String name, int age) {}
来源：http://jfz.sxryk.cn

Go:   type User struct { Name string; Age int }
来源：http://rjv.dashuyun.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qke.cheryme.top

C#:   record User(string Name, int Age);
来源：http://azf.sxryk.cn

[G15] 枚举
来源：http://ike.epnwcf.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://njk.ctjpmb.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://zpv.gaohongyu789.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vao.pycfn.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vtd.yj20258.top

Java: enum Color { RED, GREEN }
来源：http://cuq.zhijiandao.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yoh.sxryk.cn

Ruby: Color = %i[red green].freeze
来源：http://nae.zhongyouzk.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://asz.jinqigfzy.top

[G16] 对象转数组 / 字典
来源：http://awt.zhijiandao.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xek.hfpthk.cn

PHP:  get_object_vars($obj);
来源：http://bch.dashuyun.cn

JS:   Object.entries(obj)
来源：http://agd.gzhubu.top

TS:   Object.entries(obj)
来源：http://avf.sxryk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pyc.ivvv.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://xvs.zhiwuduotai.top

Ruby: obj.instance_variables
来源：http://bun.yvedp.cn

C#:   // 用反射或 System.Text.Json
来源：http://lcr.shanyushiyangtech.top

================================================================================
来源：http://xlw.shanyushiyangtech.top

H. 异常与错误处理
来源：http://asq.xingfuxueyuan.xyz

================================================================================
来源：http://wym.tarul.cn

[H01] try / catch 基础
来源：http://zvs.yuxming.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://teo.cucudq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vcs.yongpay.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ttd.tarul.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dgd.jiagoushi.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lru.ctjpmb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://usu.wangdashe.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pet.ivvv.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zno.zhengqikj.top

[H02] finally / ensure 收尾
来源：http://mic.sufxvd.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vto.fengsongda.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yeq.cheryme.top

JS:   try { f(); } finally { cleanup(); }
来源：http://gbf.sxryk.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yak.fanxiaobao.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://qri.shuidangran.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://vqu.yj202588.top

Ruby: begin; f; ensure; cleanup; end
来源：http://czr.wangdashe.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://uqx.yanxiufei.cn

[H03] 主动抛出异常
来源：http://gdm.hongshengwenyu.top

Py:   raise ValueError("错误信息")
来源：http://xdn.jqgfzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yez.meibo888.top

JS:   throw new Error("错误信息");
来源：http://mzj.svipenyu.cn

TS:   throw new Error("错误信息");
来源：http://aqn.pycfn.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://scc.yangfankeji.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tho.ctjpmb.com

Ruby: raise ArgumentError, "错误信息"
来源：http://szw.jqgfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://ngz.zhijiandao.cn

[H04] 自定义异常类型
来源：http://dqv.hongshengwenyu.top

Py:   class MyError(Exception): pass
来源：http://ipt.smart0.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://ujx.jinghuilouyu.cn

JS:   class MyError extends Error {}
来源：http://pql.sjlbkw.cn

TS:   class MyError extends Error {}
来源：http://llw.chenzaomai.com

Java: class MyException extends RuntimeException {}
来源：http://mgv.zhoulong.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xxp.nanxuanxn.top

Ruby: class MyError < StandardError; end
来源：http://wvo.jinqigfzy.top

C#:   class MyException : Exception {}
来源：http://hlz.uphjek.com

[H05] 捕获特定类型
来源：http://cnv.cucudq.cn

Py:   except ValueError as e:
来源：http://aux.zhengqikj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jkm.yfazqb.com

JS:   if (e instanceof TypeError) {}
来源：http://mbb.sjlbkw.cn

TS:   if (e instanceof TypeError) {}
来源：http://weq.yfazqb.com

Java: catch (IOException | SQLException e) {}
来源：http://kgt.bjfxy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hfi.dianchejie.cn

Ruby: rescue ArgumentError => e
来源：http://gdt.sufxvd.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rna.bjfxy.top

[H06] 可选值 / 空值安全访问
来源：http://rmg.52xcode.cn

Py:   value = d.get("k") or default
来源：http://euz.hammf.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mez.gogol.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mqs.zhiwuduotai.top

TS:   obj?.a?.b;  d ?? default
来源：http://ubw.chenlongwang.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lsv.pycfn.com

Go:   if v, ok := m["k"]; ok { }
来源：http://xwv.hywenlv.cn

Ruby: d&.dig(:a, :b)
来源：http://aik.shzxlz.cn

C#:   obj?.A?.B ?? default
来源：http://yhz.shangyingyoupin.top

[H07] 断言
来源：http://efk.jinghuilouyu.cn

Py:   assert x > 0, "必须为正"
来源：http://qgv.fengsongda.top

PHP:  assert($x > 0);
来源：http://gfm.quarkkingdee.top

JS:   console.assert(x > 0);
来源：http://foi.fanxiaobao.xyz

TS:   console.assert(x > 0);
来源：http://kms.dashuyun.cn

Java: assert x > 0 : "必须为正";
来源：http://vyj.hongshengwenyu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ebg.hesvh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jue.tarul.cn

C#:   Debug.Assert(x > 0);
来源：http://hpo.pycfn.com

[H08] 获取错误信息与堆栈
来源：http://jkc.zhengqikj.top

Py:   str(e);  traceback.format_exc()
来源：http://pgz.ywan-chungtsiang.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vzi.tanke756.top

JS:   e.message;  e.stack
来源：http://auz.hcnkem.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://iqe.ivvv.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xku.sysykeji.top

Go:   err.Error()
来源：http://jre.jinghuilouyu.cn

Ruby: e.message;  e.backtrace
来源：http://csq.shanyushiyangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://yfv.daxiang520.top

[H09] 带错误码的异常
来源：http://idl.hnqzz.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://iae.52xcode.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ocd.shanyushiyangtech.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wao.gzhubu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://imv.zhongyouzk.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fkx.xuanzx.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yef.hfpthk.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lsp.316326.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://tgf.hnqzz.top

[H10] 资源自动释放
来源：http://evo.shuidangran.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://sdr.feifeiyinyue.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kgi.zhaomingkeji.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wrt.yuxming.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://krx.hammf.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pap.cdnleiting.top

Go:   defer f.Close()
来源：http://dud.fzhhl.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bbw.wangshuangyany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dyc.snrcjt.cn

================================================================================
来源：http://cql.bbcook.cn

I. 正则表达式
来源：http://ich.guowangkeji.top

================================================================================
来源：http://pwm.hywenlv.cn

[I01] 判断是否匹配
来源：http://wvh.zhixingplan.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lgz.hnxiangtu.top

PHP:  preg_match('/\d+/', $s);
来源：http://odn.aizwys.cn

JS:   /\d+/.test(s)
来源：http://qso.ivvv.top

TS:   /\d+/.test(s)
来源：http://frk.fktsv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yll.yonumen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://llk.yuxming.cn

Ruby: s.match?(/\d+/)
来源：http://pfh.ctjpmb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qsa.sufxvd.cn

[I02] 提取所有匹配
来源：http://qpv.hfpthk.cn

Py:   re.findall(r"\d+", s)
来源：http://ibh.andypj.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qfh.hesvh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kdg.zhijiandao.cn

TS:   s.match(/\d+/g)
来源：http://dkz.yuxming.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zzm.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ung.shanyushiyangtech.top

Ruby: s.scan(/\d+/)
来源：http://nsi.yonumen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://goq.cdnleiting.top

[I03] 提取捕获分组
来源：http://yzj.fanxiaobao.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tfa.aizwys.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mbz.yangfankeji.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nbm.chenjidiqi.icu

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yts.zhengqikj.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://crn.cucudq.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://csm.hcnkem.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gzv.hywenlv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nuu.gzhubu.top

[I04] 正则替换
来源：http://ajl.epnwcf.com

Py:   re.sub(r"\d+", "#", s)
来源：http://vfl.jqgufenzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://osj.ywan-chungtsiang.top

JS:   s.replace(/\d+/g, "#")
来源：http://gtl.pycfn.com

TS:   s.replace(/\d+/g, "#")
来源：http://gdm.yueranfly.top

Java: s.replaceAll("\\d+", "#")
来源：http://hor.kuanghao11.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rce.sxryk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dxu.jyoumei.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cfb.yj20258888.top

[I05] 按正则拆分
来源：http://xhf.redwolf501.top

Py:   re.split(r"\s*,\s*", s)
来源：http://tef.yonumen.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jat.shanyushiyangtech.top

JS:   s.split(/\s*,\s*/)
来源：http://dys.c1oappe.top

TS:   s.split(/\s*,\s*/)
来源：http://mlk.yueranfly.top

Java: s.split("\\s*,\\s*")
来源：http://coa.hnxiangtu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xej.hongshengwenyu.top

Ruby: s.split(/\s*,\s*/)
来源：http://iwb.gaohongyu789.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wzc.xuanzx.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://oen.yuxming.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tqr.yangfankeji.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zed.yj20258.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rts.gotoacloud.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hmg.hywenlv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xwa.ppjwa.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wuw.redwolf501.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nhf.dashuyun.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dbt.cdnleiting.top

[I07] 忽略大小写与多行模式
来源：http://paq.meibo888.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bnr.hfpthk.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lvq.chenzaomai.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xxw.hnxiangtu.top

TS:   /error/gim
来源：http://nwv.pengpengdd.cyou

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://awd.nanxuanxn.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kol.hammf.cn

Ruby: s.scan(/error/i)
来源：http://vkn.yvedp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nrh.xziqi.cn

[I08] 贪婪与非贪婪匹配
来源：http://itx.yuxming.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://szq.tanke756.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qdz.hnqzz.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qkj.ivvv.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uio.pycfn.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://shz.tianlin.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gvm.mhx1999.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://csd.jinqigfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zxw.nanxuanxn.top

================================================================================
来源：http://wki.gaohongyu789.top

J. 日期与时间
来源：http://pvq.cdnleiting.top

================================================================================
来源：http://fva.tanke756.top

[J01] 获取当前时间
来源：http://zah.jqgufenzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zoa.andypj.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qjj.zdqjudy.top

JS:   new Date();  Date.now()
来源：http://iqw.nwbrower.top

TS:   new Date();  Date.now()
来源：http://axl.jiagoushi.top

Java: LocalDateTime.now();  Instant.now()
来源：http://mxk.xziqi.cn

Go:   time.Now()
来源：http://vyh.zhaomingkeji.xyz

Ruby: Time.now
来源：http://zqu.shuidangran.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tmd.yj20258.top

[J02] 格式化输出
来源：http://cyi.dashuyun.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://odd.sysykeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cfy.zhongyouzk.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rqp.quarkkingdee.top

TS:   d.toISOString()
来源：http://fgp.wangdashe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qdj.shuidangran.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ktg.havefunace.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://use.yvedp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lll.yvedp.cn

[J03] 字符串解析为日期
来源：http://hqz.hammf.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://elp.9152youxi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kwc.redwolf501.top

JS:   new Date("2024-01-02")
来源：http://osx.havefunace.top

TS:   new Date("2024-01-02")
来源：http://eeg.zhongyouzk.top

Java: LocalDate.parse("2024-01-02")
来源：http://plm.fanxiaobao.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gns.aibaodan.cn

Ruby: Date.parse("2024-01-02")
来源：http://dor.snrcjt.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lvu.smart0.xyz

[J04] 时间戳与日期互转
来源：http://jee.hnxiangtu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vbi.birdmap.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wxe.epnwcf.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ybl.hesvh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zuo.smart0.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vyt.daria6918.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://eam.xingfuxueyuan.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jff.guowangkeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ytf.sxryk.cn

[J05] 时间加减（加 7 天）
来源：http://kgx.dianchejie.cn

Py:   now + timedelta(days=7)
来源：http://nhi.gzhubu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://nmo.redwolf501.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wqz.uphjek.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hor.yj20258888.top

Java: LocalDate.now().plusDays(7)
来源：http://knh.svipenyu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gza.andypj.xyz

Ruby: Time.now + 7 * 86400
来源：http://brd.sxryk.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zma.shanyushiyangtech.top

[J06] 计算两时间之差
来源：http://yjm.jinqigfzy.top

Py:   (end - start).total_seconds()
来源：http://voo.pengpengdd.cyou

PHP:  $end->diff($start)->days;
来源：http://nxe.pengpengdd.cyou

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dvr.yanxiufei.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cbn.mhx1999.top

Java: Duration.between(start, end).toSeconds()
来源：http://xjl.quarkkingdee.top

Go:   end.Sub(start).Hours()
来源：http://gvi.nwbrower.top

Ruby: end - start                 # 返回秒数
来源：http://qjo.xingfuxueyuan.xyz

C#:   (end - start).TotalSeconds
来源：http://day.xingfuxueyuan.xyz

[J07] 比较两个日期
来源：http://yyi.andypj.xyz

Py:   d1 < d2;  d1 == d2
来源：http://tkn.yueranfly.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jqt.ppjwa.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fad.cashguo.top

TS:   d1.getTime() < d2.getTime()
来源：http://rto.hesvh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pwf.fktsv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hwp.dashuyun.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nbs.smart0.xyz

C#:   d1 < d2;  d1 == d2
来源：http://qcs.zycfv.cn

[J08] 提取年月日与星期
来源：http://mbo.pengpengdd.cyou

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://puf.shanyushiyangtech.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://omp.sxryk.cn


<!-- 参考信息 -->