代发 wailian999

[Q78] 当前时间
来源：http://god.ctjpmb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wso.hesvh.cn

[Q79] 字符串拼接
来源：http://yra.ctjpmb.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bxq.hysaishi.cn

[Q80] 字符串截取
来源：http://kje.guannengcc.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oxo.shanyushiyangtech.top

[Q81] 字符串替换
来源：http://tkw.smart0.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uwd.birdmap.top

[Q82] 字符长度与字节长度
来源：http://clb.jinqigufen.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rlh.yangfankeji.com

[Q83] 大小写转换
来源：http://luw.hnqzz.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://frf.shangyingyoupin.top

[Q84] 去除首尾空格
来源：http://ovr.gogol.net.cn

SELECT TRIM(name) FROM users;
来源：http://hqa.daria6918.cn

[Q85] 数值取整
来源：http://lhl.andypj.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fxz.cheryme.top

[Q86] 读取 JSON 字段
来源：http://cde.bbcook.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wtn.cashguo.top

[Q87] JSON 字段做条件
来源：http://jtp.cheryme.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ada.jlsjyb.cn

[Q88] 行转列（条件聚合）
来源：http://bhq.jinghuilouyu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wil.sjlbkw.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ctk.chenlongwang.top

[Q89] 判断表是否存在
来源：http://cpv.aizwys.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yms.tarul.cn

[Q90] 生成序号列
来源：http://azv.hnqzz.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ilk.zhijiandao.cn

================================================================================
来源：http://ucy.cheryme.top

R. Bash 专题
来源：http://hst.yuanzhike.top

================================================================================
来源：http://hnk.ydjk.org.cn

[R01] shebang 与严格模式
来源：http://gpk.shzxlz.cn

#!/usr/bin/env bash
来源：http://tix.cqqwz.cn

set -euo pipefail
来源：http://ypj.zycfv.cn

[R02] 变量赋值与使用
来源：http://bmu.meibo888.top

name="Tom"; echo "$name"
来源：http://uwa.pengpengdd.cyou

[R03] 只读变量
来源：http://bqv.yj202588.top

readonly PI=3.14
来源：http://fzr.cheryme.top

[R04] 位置参数
来源：http://vzh.yj20258888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vqa.zhengqikj.top

[R05] 参数默认值
来源：http://kjn.bjfxy.top

name="${1:-default}"
来源：http://kdc.wangdashe.top

[R06] 判断命令是否存在
来源：http://sdt.vehdjk.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://snr.hcnkem.com

[R07] if 判断文件
来源：http://afr.hysaishi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qew.guowangkeji.top

[R08] 数值比较
来源：http://lss.shangyingyoupin.top

if (( a > b )); then echo "a 更大"; fi
来源：http://hck.sweek.top

[R09] 字符串比较
来源：http://nqf.svipenyu.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lxv.yuxming.cn

[R10] 正则匹配
来源：http://cll.ydzc1.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ytu.shzxlz.cn

[R11] case 多分支
来源：http://wqa.zhongyouzk.top

case "$1" in
来源：http://tsb.zhaomingkeji.xyz

start) echo "启动" ;;
来源：http://olf.iojbl.cn

stop)  echo "停止" ;;
来源：http://jox.uphjek.com

*)     echo "未知命令" ;;
来源：http://tei.cheryme.top

esac
来源：http://paz.shangyingyoupin.top

[R12] for 遍历文件
来源：http://kci.shzxlz.cn

for f in *.txt; do echo "$f"; done
来源：http://icj.jyoumei.cn

[R13] for 计数循环
来源：http://jor.gogol.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://vmv.fzhhl.top

[R14] C 风格 for
来源：http://lml.jyoumei.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bzd.52xcode.cn

[R15] while 逐行读文件
来源：http://fno.meibo888.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rlr.hysaishi.cn

[R16] until 等待条件
来源：http://rmy.aibaodan.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hhx.jinghuilouyu.cn

[R17] 数组定义与取值
来源：http://iuz.redwolf501.top

arr=(a b c); echo "${arr[0]}"
来源：http://ndb.ppjwa.cn

[R18] 遍历数组
来源：http://vfh.iojbl.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kab.xylfe.cn

[R19] 数组长度
来源：http://cby.nanxinkj.top

echo "${#arr[@]}"
来源：http://sfa.xylfe.cn

[R20] 关联数组（字典）
来源：http://lga.andypj.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zmi.daxiang520.top

[R21] 字符串长度
来源：http://xen.yuxming.cn

echo "${#s}"
来源：http://sax.sysykeji.top

[R22] 截取子串
来源：http://rpy.fengsongda.top

echo "${s:0:5}"
来源：http://bnl.ctjpmb.com

[R23] 字符串替换
来源：http://exr.sxryk.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://poy.cdnleiting.top

[R24] 大小写转换
来源：http://pyf.gogol.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://iuh.hnxiangtu.top

[R25] 去后缀 / 去前缀
来源：http://utk.vqdsnc.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cgo.jiagoushi.top

[R26] 命令替换
来源：http://ozp.ivvv.top

now=$(date +%F); echo "$now"
来源：http://hut.fanxiaobao.xyz

[R27] 算术展开
来源：http://ivm.ivvv.top

echo $((1 + 2 * 3))
来源：http://abv.smart0.xyz

[R28] 浮点运算
来源：http://mxp.hfpthk.cn

echo "scale=2; 10/3" | bc
来源：http://eph.316326.xyz

[R29] 定义函数
来源：http://kog.fanxiaobao.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pjq.aizwys.cn

[R30] 函数返回状态码
来源：http://dpc.sysykeji.top

f() { return 0; }; f || echo "失败了"
来源：http://nus.xylfe.cn

[R31] 局部变量
来源：http://kkj.ydjk.org.cn

f() { local x=1; echo "$x"; }
来源：http://ipx.chenzaomai.com

[R32] 参数个数校验
来源：http://hls.vqdsnc.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ubx.yanxiufei.cn

[R33] 捕获错误并提示行号
来源：http://vxu.hnxiangtu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gka.jianghu66.top

[R34] 退出时清理
来源：http://ufb.gotoacloud.top

trap 'rm -f "$tmp"' EXIT
来源：http://vdf.cheryme.top

[R35] 后台执行并等待
来源：http://vnv.cashguo.top

sleep 5 & pid=$!; wait "$pid"
来源：http://doa.jinghuilouyu.cn

[R36] 并发执行多个任务
来源：http://wpv.hnxiangtu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xne.hesvh.cn

[R37] 把输出赋给变量
来源：http://lsh.havefunace.top

files=$(ls -1)
来源：http://phd.ppjwa.cn

[R38] 管道串联
来源：http://txc.sufxvd.cn

cat a.txt | grep -i error | wc -l
来源：http://ydn.dashuyun.cn

[R39] 重定向标准输出与错误
来源：http://ewy.cheryme.top

cmd > out.log 2>&1
来源：http://ncs.sjlbkw.cn

[R40] 追加写日志
来源：http://faz.ydjk.org.cn

echo "log" >> out.log
来源：http://cmx.yfazqb.com

[R41] 丢弃输出
来源：http://axc.cheryme.top

cmd >/dev/null 2>&1
来源：http://izm.xziqi.cn

[R42] 输入重定向
来源：http://cfj.chenlongwang.top

wc -l < a.txt
来源：http://yqa.xuanzx.com

[R43] 按名字查找文件
来源：http://cvp.redwolf501.top

find . -name "*.log" -type f
来源：http://nkw.cdnleiting.top

[R44] 按修改时间查找
来源：http://fyi.ydjk.org.cn

find . -mtime -7 -type f
来源：http://npu.daxiang520.top

[R45] 批量删除
来源：http://nqu.gzhubu.top

find . -name "*.tmp" -delete
来源：http://pxq.fehbvm.com

[R46] 递归替换文件内容
来源：http://ljj.snrcjt.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qms.yfazqb.com

[R47] sed 单行替换
来源：http://kgx.yj20258.top

sed -i 's/foo/bar/g' a.txt
来源：http://jdo.feifeiyinyue.top

[R48] awk 取指定列
来源：http://tcm.wangshuangyany.cn

awk '{print $1, $3}' a.txt
来源：http://jaa.gaohongyu789.top

[R49] awk 带条件
来源：http://flw.cheryme.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://aql.gaohongyu789.top

[R50] awk 求和
来源：http://sgr.dianchejie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cwe.gzhubu.top

[R51] 排序去重取前几
来源：http://wna.cashguo.top

sort a.txt | uniq -c | sort -rn | head
来源：http://sab.wangshuangyany.cn

[R52] 统计行数
来源：http://bji.zdqjudy.top

wc -l a.txt
来源：http://agn.wangshuangyany.cn

[R53] 查看文件头与实时尾
来源：http://fsr.xuanzx.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kfu.nanxinkj.top

[R54] 比较两个文件
来源：http://feb.fzhhl.top

diff a.txt b.txt
来源：http://otl.vqdsnc.cn

[R55] 压缩与解压
来源：http://ukp.fengsongda.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yrp.hongshengwenyu.top

[R56] 远程拷贝
来源：http://ump.9152youxi.cn

scp file user@host:/path/
来源：http://vho.sjlbkw.cn

[R57] 远程执行命令
来源：http://zjw.yongpay.top

ssh user@host 'uptime'
来源：http://fol.vehdjk.com

[R58] 下载文件
来源：http://lap.fzhhl.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hct.shangyingyoupin.top

[R59] 发 POST JSON
来源：http://hhf.shanyushiyangkeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vbe.jiagoushi.top

[R60] 只看 HTTP 状态码
来源：http://gsj.ivvv.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://aeu.sxryk.cn

[R61] 磁盘占用
来源：http://mhi.tarul.cn

df -h;  du -sh *
来源：http://bso.bjfxy.top

[R62] 找最占空间的文件
来源：http://qco.hesvh.cn

du -ah . | sort -rh | head -10
来源：http://sbg.yuanzhike.top

[R63] 内存与进程
来源：http://xku.cashguo.top

free -h;  ps aux | grep nginx
来源：http://lss.tian-w.cn

[R64] 结束进程
来源：http://kgx.yuxming.cn

kill -9 $(pgrep -f app.py)
来源：http://pqn.cqqwz.cn

[R65] 查看端口占用
来源：http://zhz.nanxuanxn.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://adx.xinyue.icu

[R66] 定时任务
来源：http://ekd.yueranfly.top

crontab -e;  crontab -l
来源：http://pyt.pengpengdd.cyou

[R67] 生成随机十六进制串
来源：http://yyo.gzhubu.top

openssl rand -hex 16
来源：http://awj.snrcjt.cn

[R68] 计算文件校验值
来源：http://bqo.shzxlz.cn

sha256sum a.txt;  md5sum a.txt
来源：http://oix.shangyingyoupin.top

[R69] 生成随机密码
来源：http://gbc.quarkkingdee.top

head -c 16 /dev/urandom | base64
来源：http://tlh.cashguo.top

[R70] 时间戳与互转
来源：http://pqp.havefunace.top

date +%s;  date -d @1700000000
来源：http://rqu.fzhhl.top

[R71] 日期格式化
来源：http://rag.daria6918.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zum.gzhubu.top

[R72] 等待端口就绪
来源：http://qil.xziqi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rvf.haohaochexian.top

[R73] 分割大日志
来源：http://kif.bjfxy.top

split -l 1000 big.log part_
来源：http://wrt.vqdsnc.cn

[R74] 批量重命名
来源：http://oot.smart0.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xun.tarul.cn

[R75] 导出环境变量
来源：http://rob.havefunace.top

export PATH="$HOME/bin:$PATH"
来源：http://blq.iojbl.cn

[R76] 使用临时文件
来源：http://bmd.dashuyun.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ilf.cheryme.top

[R77] 读取用户输入
来源：http://xwv.epnwcf.com

read -rp "请输入: " ans
来源：http://fbj.hfpthk.cn

[R78] 交互式菜单
来源：http://ayb.smart0.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://zdw.ehwqpu.com

[R79] 解析命令行选项
来源：http://eul.meibo888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vne.hfpthk.cn

[R80] 查看脚本执行耗时
来源：http://yno.hcnkem.com

time ./run.sh
来源：http://ayx.redwolf501.top

================================================================================
来源：http://jqw.hysaishi.cn

S. C / C++ 专题
来源：http://oll.cashguo.top

================================================================================
来源：http://gmt.sxryk.cn

[S01] C：Hello World
来源：http://llq.vqdsnc.cn

#include <stdio.h>
来源：http://lef.smart0.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://ydg.pengpengdd.cyou

[S02] C：变量与格式化输出
来源：http://tmc.hammf.cn

int a = 10; printf("%d\n", a);
来源：http://een.wangshuangyany.cn

[S03] C：读入整数
来源：http://vqm.yuanzhike.top

int x; scanf("%d", &x);
来源：http://jjv.zhixingplan.top

[S04] C：字符串复制
来源：http://khn.andypj.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://yhn.zhoulong.xyz

[S05] C：字符串长度
来源：http://mzc.shanyushiyangkeji.top

strlen(s)
来源：http://uzs.wangshuangyany.cn

[S06] C：字符串比较
来源：http://cmp.yanxiufei.cn

strcmp(a, b) == 0
来源：http://ozu.ydjk.org.cn

[S07] C：数组遍历求和
来源：http://qvl.bjfxy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xfm.shzxlz.cn

[S08] C：动态内存分配与释放
来源：http://qqh.wangdashe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vhy.jianghu66.top

[S09] C：结构体定义与初始化
来源：http://wrd.cucudq.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://usc.daxiang520.top

[S10] C：指针与解引用
来源：http://eob.c1oappe.top

int *p = &a;  *p = 5;
来源：http://wfg.ctjpmb.com

[S11] C：逐行读文件
来源：http://xno.9152youxi.cn

FILE *f = fopen("a.txt", "r");
来源：http://myk.jianghu66.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://hxy.jlsjyb.cn

fclose(f);
来源：http://tvc.yueranfly.top

[S12] C：写文件
来源：http://vyl.zhaomingkeji.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rxf.yj202588.top

[S13] C：宏定义
来源：http://dgu.hysaishi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ivu.ydjk.org.cn

[S14] C：枚举
来源：http://ckj.fanxiaobao.xyz

enum Color { RED, GREEN, BLUE };
来源：http://uxg.ehwqpu.com

[S15] C：类型转换
来源：http://ejl.hnxiangtu.top

(double) a / b
来源：http://wzi.yuxming.cn

[S16] C：位操作置位
来源：http://nwj.fehbvm.com

x |= (1 << 3);
来源：http://wrk.jqgfzy.top

[S17] C：安全拼接字符串
来源：http://mch.52xcode.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sai.daria6918.cn

[S18] C：命令行参数
来源：http://hnk.daxiang520.top

int main(int argc, char **argv)
来源：http://fps.haohaochexian.top

[S19] C：快速排序
来源：http://wzi.yueranfly.top

qsort(a, n, sizeof(int), cmp);
来源：http://uuf.redwolf501.top

[S20] C：二分查找
来源：http://cfg.sufxvd.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ehm.xingfuxueyuan.xyz

[S21] C：字符类别判断
来源：http://guc.wangshuangyany.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://age.mhx1999.top

[S22] C：字符串转数字
来源：http://upr.yueranfly.top

atoi("42");  strtod("3.14", NULL);
来源：http://hox.snrcjt.cn

[S23] C：随机数
来源：http://eko.hongshengwenyu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://kug.uphjek.com

[S24] C：获取本地时间
来源：http://dwc.xylfe.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tzy.shuidangran.top

[S25] C：内存拷贝
来源：http://hxv.jlsjyb.cn

memcpy(dst, src, n);
来源：http://qfm.9152youxi.cn

[S26] C：内存清零
来源：http://amo.kuanghao11.cn

memset(a, 0, sizeof a);
来源：http://poo.nanxuanxn.top

[S27] C：定义常量
来源：http://mfn.zhiwuduotai.top

const double PI = 3.14159;
来源：http://lgr.shangyingyoupin.top

[S28] C：静态变量
来源：http://rvl.jqgufenzy.top

static int counter = 0;
来源：http://juv.jinyuanbaomall.cn

[S29] C：变参函数
来源：http://fzi.guowangkeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kxs.sxryk.cn

[S30] C：头文件保护
来源：http://aew.pycfn.com

#ifndef X_H
来源：http://qbq.jlsjyb.cn

#define X_H
来源：http://dly.jianghu66.top

#endif
来源：http://dql.xinyue.icu

[S31] C++：Hello World
来源：http://kbm.shanyushiyangtech.top

#include <iostream>
来源：http://fwx.cucudq.cn

int main() { std::cout << "Hello\n"; }
来源：http://bdv.jianghu66.top

[S32] C++：字符串
来源：http://rlo.ybcxt.top

std::string s = "hi";  s += "!";
来源：http://lqm.ydzc1.top

[S33] C++：vector 增删
来源：http://fwd.hnxiangtu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ppj.yj20258888.top

[S34] C++：遍历 vector
来源：http://yeo.chenlongwang.top

for (auto &x : v) { std::cout << x; }
来源：http://khv.vqdsnc.cn

[S35] C++：map
来源：http://jvn.hywenlv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bfh.hfpthk.cn

[S36] C++：unordered_map
来源：http://kbj.jinghuilouyu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://axi.xziqi.cn

[S37] C++：set
来源：http://mfq.haohaochexian.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xat.yanxiufei.cn

[S38] C++：排序
来源：http://rak.daria6918.cn

std::sort(v.begin(), v.end());
来源：http://oyr.sjlbkw.cn

[S39] C++：自定义比较器排序
来源：http://yeo.jyoumei.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sdh.zhixingplan.top

[S40] C++：查找元素
来源：http://yyq.tarul.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xpx.kuanghao11.cn

[S41] C++：类与构造函数
来源：http://rvm.bbcook.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ida.gogol.net.cn

[S42] C++：继承与虚函数
来源：http://vwl.meibo888.top

class B : public Base { public: void f() override {} };
来源：http://nzh.cashguo.top

[S43] C++：智能指针
来源：http://dut.gzhubu.top

auto p = std::make_unique<int>(5);
来源：http://txl.jlsjyb.cn

[S44] C++：引用传参
来源：http://xda.havefunace.top

void inc(int &x) { ++x; }
来源：http://pot.chenzaomai.com

[S45] C++：lambda
来源：http://ijl.jinyuanbaomall.cn

auto add = [](int a, int b) { return a + b; };
来源：http://uel.dianchejie.cn

[S46] C++：函数模板
来源：http://ngq.tanke756.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ctc.yongpay.top

[S47] C++：结构化绑定遍历
来源：http://ktw.yvedp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ajx.0kj1m.cn

[S48] C++：逐行读文件
来源：http://wgn.yuanzhike.top

std::ifstream in("a.txt");  std::string line;
来源：http://ijy.zdbjq.cn


<!-- 参考信息 -->