代发 wailian999

[G10] 访问控制
来源：http://zos.guannengcc.top

Py:   约定 _protected / __private（不强制）
来源：http://hfq.daria6918.cn

PHP:  public / protected / private
来源：http://luk.andypj.xyz

JS:   #private 字段；其余公开
来源：http://wws.zhijiandao.cn

TS:   public / protected / private
来源：http://bdk.quarkkingdee.top

Java: public / protected / private / 默认包级
来源：http://icb.andypj.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://vok.yfazqb.com

Ruby: public / protected / private
来源：http://ntt.zhiwuduotai.top

C#:   public / protected / private / internal
来源：http://ode.xinyue.icu

[G11] getter / setter
来源：http://crq.xylfe.cn

Py:   @property 与 @x.setter
来源：http://ude.yj202588.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ghv.tanke756.top

JS:   get name() { return this._name; }
来源：http://fvq.yanxiufei.cn

TS:   get name(): string { return this._name; }
来源：http://afx.aizwys.cn

Java: public String getName() { return name; }
来源：http://ase.hongshengwenyu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jhs.jinqigufen.top

Ruby: attr_accessor :name
来源：http://bgl.gotoacloud.top

C#:   public string Name { get; set; }
来源：http://iei.ppjwa.cn

[G12] 对象转字符串
来源：http://myk.zhongyouzk.top

Py:   def __str__(self): return self.name
来源：http://rsi.cucudq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://isg.xziqi.cn

JS:   toString() { return this.name; }
来源：http://qeo.jinyuanbaomall.cn

TS:   toString(): string { return this.name; }
来源：http://lpd.tianlin.xyz

Java: @Override public String toString() { return name; }
来源：http://jle.nwbrower.top

Go:   func (u User) String() string { return u.Name }
来源：http://toy.jianghu66.top

Ruby: def to_s; @name; end
来源：http://hhf.shzxlz.cn

C#:   public override string ToString() => Name;
来源：http://ent.yangfankeji.com

[G13] 判断对象类型
来源：http://tpj.bbcook.cn

Py:   isinstance(u, User)
来源：http://lwo.hesvh.cn

PHP:  $u instanceof User
来源：http://yho.cashguo.top

JS:   u instanceof User
来源：http://sxr.yangfankeji.com

TS:   u instanceof User
来源：http://tpu.redwolf501.top

Java: u instanceof User
来源：http://xpe.birdmap.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://lby.ppjwa.cn

Ruby: u.is_a?(User)
来源：http://gcz.iojbl.cn

C#:   u is User
来源：http://sif.uphjek.com

[G14] 数据类 / record
来源：http://nfo.feifeiyinyue.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lbc.haohaochexian.top

PHP:  // 用 readonly 属性模拟
来源：http://yfr.jianghu66.top

JS:   // 无内置：普通类或对象字面量
来源：http://oif.cucudq.cn

TS:   type User = { name: string; age: number };
来源：http://zfk.dashuyun.cn

Java: record User(String name, int age) {}
来源：http://nkv.dianchejie.cn

Go:   type User struct { Name string; Age int }
来源：http://urk.fehbvm.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vwg.feifeiyinyue.top

C#:   record User(string Name, int Age);
来源：http://kqo.xingfuxueyuan.xyz

[G15] 枚举
来源：http://dbv.sufxvd.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jhr.iojbl.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xxg.pycfn.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://buz.shzxlz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mee.daria6918.cn

Java: enum Color { RED, GREEN }
来源：http://kfg.cashguo.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gga.ivvv.top

Ruby: Color = %i[red green].freeze
来源：http://vxq.shuidangran.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lpv.0kj1m.cn

[G16] 对象转数组 / 字典
来源：http://llb.yfazqb.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kkw.bjfxy.top

PHP:  get_object_vars($obj);
来源：http://zjo.zycfv.cn

JS:   Object.entries(obj)
来源：http://cqf.chenjidiqi.icu

TS:   Object.entries(obj)
来源：http://mis.gzhubu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://awa.iojbl.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://twd.hnxiangtu.top

Ruby: obj.instance_variables
来源：http://eyh.shanyushiyangkeji.top

C#:   // 用反射或 System.Text.Json
来源：http://itr.ywan-chungtsiang.top

================================================================================
来源：http://tnx.yanxiufei.cn

H. 异常与错误处理
来源：http://vjk.ppjwa.cn

================================================================================
来源：http://yex.jinghuilouyu.cn

[H01] try / catch 基础
来源：http://ppk.zhongyouzk.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gmp.meibo888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vpx.yanxiufei.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yaq.fehbvm.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hma.cashguo.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://crx.haohaochexian.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://toa.sysykeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kws.jinyuanbaomall.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://aqd.havefunace.top

[H02] finally / ensure 收尾
来源：http://mcq.yfazqb.com

Py:   try: f()⏎finally: cleanup()
来源：http://dac.316326.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://iam.zhengqikj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://umv.zdqjudy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://fsq.wangshuangyany.cn

Java: try { f(); } finally { cleanup(); }
来源：http://guh.xziqi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ryh.jinqigufen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qfz.daxiang520.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://wdj.shanyushiyangkeji.top

[H03] 主动抛出异常
来源：http://jpb.nanxinkj.top

Py:   raise ValueError("错误信息")
来源：http://qhb.jqgfzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gcg.sjlbkw.cn

JS:   throw new Error("错误信息");
来源：http://phb.nanxinkj.top

TS:   throw new Error("错误信息");
来源：http://wfr.hfpthk.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://axu.nanxinkj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wrb.chenlongwang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hjk.gaohongyu789.top

C#:   throw new ArgumentException("错误信息");
来源：http://zrm.xingfuxueyuan.xyz

[H04] 自定义异常类型
来源：http://pgy.hnxiangtu.top

Py:   class MyError(Exception): pass
来源：http://inh.yongpay.top

PHP:  class MyError extends RuntimeException {}
来源：http://tnk.cucudq.cn

JS:   class MyError extends Error {}
来源：http://wim.daria6918.cn

TS:   class MyError extends Error {}
来源：http://erv.wangdashe.top

Java: class MyException extends RuntimeException {}
来源：http://gbo.ehwqpu.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://urd.sweek.top

Ruby: class MyError < StandardError; end
来源：http://rws.ydzc1.top

C#:   class MyException : Exception {}
来源：http://rap.iojbl.cn

[H05] 捕获特定类型
来源：http://tzx.jinyuanbaomall.cn

Py:   except ValueError as e:
来源：http://emr.sxryk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lse.fanxiaobao.xyz

JS:   if (e instanceof TypeError) {}
来源：http://ilg.cucudq.cn

TS:   if (e instanceof TypeError) {}
来源：http://inq.shanyushiyangtech.top

Java: catch (IOException | SQLException e) {}
来源：http://zjd.yvedp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fdi.shzxlz.cn

Ruby: rescue ArgumentError => e
来源：http://exj.zdqjudy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://khk.yuanzhike.top

[H06] 可选值 / 空值安全访问
来源：http://dvf.zhongyouzk.top

Py:   value = d.get("k") or default
来源：http://cno.meibo888.top

PHP:  $v = $d["k"] ?? null;
来源：http://azh.cheryme.top

JS:   obj?.a?.b;  d ?? default
来源：http://rvh.hnqzz.top

TS:   obj?.a?.b;  d ?? default
来源：http://gou.jlsjyb.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qmd.cdnleiting.top

Go:   if v, ok := m["k"]; ok { }
来源：http://kzp.bbcook.cn

Ruby: d&.dig(:a, :b)
来源：http://tek.jinqigufen.top

C#:   obj?.A?.B ?? default
来源：http://shs.jianghu66.top

[H07] 断言
来源：http://xpw.yfazqb.com

Py:   assert x > 0, "必须为正"
来源：http://des.vqdsnc.cn

PHP:  assert($x > 0);
来源：http://vlj.xziqi.cn

JS:   console.assert(x > 0);
来源：http://jfx.cucudq.cn

TS:   console.assert(x > 0);
来源：http://eak.dianchejie.cn

Java: assert x > 0 : "必须为正";
来源：http://hxm.yfazqb.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://laa.sufxvd.cn

Ruby: raise "必须为正" unless x > 0
来源：http://uhx.pycfn.com

C#:   Debug.Assert(x > 0);
来源：http://pms.ctjpmb.com

[H08] 获取错误信息与堆栈
来源：http://bbl.zhiwuduotai.top

Py:   str(e);  traceback.format_exc()
来源：http://xhy.hywenlv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hqn.cqqwz.cn

JS:   e.message;  e.stack
来源：http://nlq.dianchejie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ogj.yvedp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bnb.tianlin.xyz

Go:   err.Error()
来源：http://qzb.ywan-chungtsiang.top

Ruby: e.message;  e.backtrace
来源：http://dxl.ctjpmb.com

C#:   e.Message;  e.StackTrace
来源：http://qep.daria6918.cn

[H09] 带错误码的异常
来源：http://tvr.yonumen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ghn.hesvh.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://uvc.ehwqpu.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ggh.yfazqb.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://raa.wangshuangyany.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://too.jinghuilouyu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vke.jiagoushi.top

Ruby: raise MyError.new("fail", 500)
来源：http://yfj.pycfn.com

C#:   // 自定义异常类中加 Code 属性
来源：http://isy.gogol.net.cn

[H10] 资源自动释放
来源：http://wnz.hongshengwenyu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://kis.nanxinkj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://adh.meibo888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fdr.hongshengwenyu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fhv.nanxinkj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tsf.nanxuanxn.top

Go:   defer f.Close()
来源：http://pzt.bbcook.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://saj.jiagoushi.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oud.wangshuangyany.cn

================================================================================
来源：http://lwj.fanxiaobao.xyz

I. 正则表达式
来源：http://rvy.xinyue.icu

================================================================================
来源：http://hec.jiagoushi.top

[I01] 判断是否匹配
来源：http://opx.chenjidiqi.icu

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rlz.hammf.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sww.ivvv.top

JS:   /\d+/.test(s)
来源：http://gzc.jinghuilouyu.cn

TS:   /\d+/.test(s)
来源：http://vwv.meibo888.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gsv.yonumen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nki.chenlongwang.top

Ruby: s.match?(/\d+/)
来源：http://axw.shangyingyoupin.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ogv.zhengqikj.top

[I02] 提取所有匹配
来源：http://lhs.svipenyu.cn

Py:   re.findall(r"\d+", s)
来源：http://jkx.shuidangran.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ioj.haohaochexian.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qeq.ywan-chungtsiang.top

TS:   s.match(/\d+/g)
来源：http://qcb.fktsv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://axf.daxiang520.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tqt.tanke756.top

Ruby: s.scan(/\d+/)
来源：http://cud.ydjk.org.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bgf.yvedp.cn

[I03] 提取捕获分组
来源：http://kww.havefunace.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rdg.cqqwz.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cpy.cqqwz.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cyr.nanxuanxn.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xva.yj202588.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vib.hnqzz.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vrn.pycfn.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wtx.zycfv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ulm.jianghu66.top

[I04] 正则替换
来源：http://kdz.kuanghao11.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bnj.guowangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nmf.jinqigfzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://bbn.meibo888.top

TS:   s.replace(/\d+/g, "#")
来源：http://sty.jinyuanbaomall.cn

Java: s.replaceAll("\\d+", "#")
来源：http://isf.cashguo.top

Go:   re.ReplaceAllString(s, "#")
来源：http://rap.vqdsnc.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lwt.cashguo.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uaj.yanxiufei.cn

[I05] 按正则拆分
来源：http://avp.redwolf501.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ijy.bjfxy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jyn.52xcode.cn

JS:   s.split(/\s*,\s*/)
来源：http://oys.shuidangran.top

TS:   s.split(/\s*,\s*/)
来源：http://uxm.guannengcc.top

Java: s.split("\\s*,\\s*")
来源：http://dao.bbcook.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kpl.chenlongwang.top

Ruby: s.split(/\s*,\s*/)
来源：http://dus.hesvh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://omj.xylfe.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vko.ywan-chungtsiang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://erx.havefunace.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qad.jqgfzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fvw.haohaochexian.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ava.fengsongda.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ype.yvedp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sng.fengsongda.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vde.guowangkeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zcq.ybcxt.top

[I07] 忽略大小写与多行模式
来源：http://wdz.vqdsnc.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gyt.nanxuanxn.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rcu.cdnleiting.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ovg.shanyushiyangtech.top

TS:   /error/gim
来源：http://wgr.birdmap.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jpu.jlsjyb.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qdo.hywenlv.cn

Ruby: s.scan(/error/i)
来源：http://kor.gotoacloud.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lqa.kuanghao11.cn

[I08] 贪婪与非贪婪匹配
来源：http://edi.0kj1m.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qbf.ywan-chungtsiang.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tgt.andypj.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vff.redwolf501.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pab.redwolf501.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ufj.smart0.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wqp.gaohongyu789.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qri.daria6918.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ztq.yuxming.cn

================================================================================
来源：http://ugq.ehwqpu.com

J. 日期与时间
来源：http://uyx.smart0.xyz

================================================================================
来源：http://nvy.meibo888.top

[J01] 获取当前时间
来源：http://lhx.zhixingplan.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ebh.epnwcf.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zky.ppjwa.cn

JS:   new Date();  Date.now()
来源：http://sgy.tianlin.xyz

TS:   new Date();  Date.now()
来源：http://jdj.haohaochexian.top

Java: LocalDateTime.now();  Instant.now()
来源：http://sso.yj20258888.top

Go:   time.Now()
来源：http://pqe.ctjpmb.com

Ruby: Time.now
来源：http://yra.zdqjudy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bqj.epnwcf.com

[J02] 格式化输出
来源：http://cby.tianlin.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blb.smart0.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vtl.hnxiangtu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ssu.shzxlz.cn

TS:   d.toISOString()
来源：http://cfv.hongshengwenyu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://utw.gzhubu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jrx.zdqjudy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jpd.jlsjyb.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tqc.shzxlz.cn

[J03] 字符串解析为日期
来源：http://znz.nwbrower.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vck.hfpthk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://usq.jqgfzy.top

JS:   new Date("2024-01-02")
来源：http://htt.andypj.xyz

TS:   new Date("2024-01-02")
来源：http://czv.zycfv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wxh.shuidangran.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://frg.svipenyu.cn

Ruby: Date.parse("2024-01-02")
来源：http://uxn.9152youxi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jhp.cdnleiting.top

[J04] 时间戳与日期互转
来源：http://uov.pengpengdd.cyou

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lxv.sysykeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lij.0kj1m.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ogj.chenlongwang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://bzd.shzxlz.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lyy.xuetiantiany.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wds.0kj1m.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tvc.gzhubu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cdm.tianlin.xyz

[J05] 时间加减（加 7 天）
来源：http://kew.jlsjyb.cn

Py:   now + timedelta(days=7)
来源：http://uwg.shanyushiyangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://gno.xinyue.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ajw.shzxlz.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hll.cheryme.top

Java: LocalDate.now().plusDays(7)
来源：http://gsk.tarul.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wzo.cashguo.top

Ruby: Time.now + 7 * 86400
来源：http://dvd.ydzc1.top

C#:   DateTime.Now.AddDays(7)
来源：http://zze.cheryme.top

[J06] 计算两时间之差
来源：http://fyu.vqdsnc.cn

Py:   (end - start).total_seconds()
来源：http://lsw.pycfn.com

PHP:  $end->diff($start)->days;
来源：http://umf.wangdashe.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ibn.hammf.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://enc.hcnkem.com

Java: Duration.between(start, end).toSeconds()
来源：http://ohv.pengpengdd.cyou

Go:   end.Sub(start).Hours()
来源：http://ott.bbcook.cn

Ruby: end - start                 # 返回秒数
来源：http://rcj.c1oappe.top

C#:   (end - start).TotalSeconds
来源：http://nre.yfazqb.com

[J07] 比较两个日期
来源：http://etp.xinyue.icu

Py:   d1 < d2;  d1 == d2
来源：http://yaq.jqgfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://krq.pycfn.com

JS:   d1.getTime() < d2.getTime()
来源：http://xiw.yanxiufei.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yni.zhaomingkeji.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vwt.shuidangran.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rps.yangfankeji.com

Ruby: d1 < d2;  d1 == d2
来源：http://jkb.gotoacloud.top

C#:   d1 < d2;  d1 == d2
来源：http://pln.xuanzx.com

[J08] 提取年月日与星期
来源：http://jik.fktsv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dgq.zhengqikj.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rjw.cqqwz.cn


<!-- 参考信息 -->