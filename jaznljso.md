代发 wailian999

[Q78] 当前时间
来源：http://bzd.ydzc1.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ojj.xziqi.cn

[Q79] 字符串拼接
来源：http://msy.hnxiangtu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yah.vqdsnc.cn

[Q80] 字符串截取
来源：http://ehc.fktsv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rna.ctjpmb.com

[Q81] 字符串替换
来源：http://ajp.hesvh.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gqy.yangfankeji.com

[Q82] 字符长度与字节长度
来源：http://kzy.sxryk.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lpj.nanxinkj.top

[Q83] 大小写转换
来源：http://npd.guowangkeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fox.tianlin.xyz

[Q84] 去除首尾空格
来源：http://jrr.xuanzx.com

SELECT TRIM(name) FROM users;
来源：http://znw.52xcode.cn

[Q85] 数值取整
来源：http://wjj.aizwys.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jsi.chenzaomai.com

[Q86] 读取 JSON 字段
来源：http://bae.daria6918.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tgp.cqqwz.cn

[Q87] JSON 字段做条件
来源：http://zzc.gogol.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zei.hcnkem.com

[Q88] 行转列（条件聚合）
来源：http://egq.fehbvm.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fyq.yanxiufei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nuy.svipenyu.cn

[Q89] 判断表是否存在
来源：http://mdw.zhongyouzk.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://edl.fengsongda.top

[Q90] 生成序号列
来源：http://fkw.zycfv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tcl.uphjek.com

================================================================================
来源：http://msh.redwolf501.top

R. Bash 专题
来源：http://efa.gotoacloud.top

================================================================================
来源：http://qgw.yongpay.top

[R01] shebang 与严格模式
来源：http://smz.quarkkingdee.top

#!/usr/bin/env bash
来源：http://gjf.jinghuilouyu.cn

set -euo pipefail
来源：http://dpz.zdqjudy.top

[R02] 变量赋值与使用
来源：http://vuu.jqgufenzy.top

name="Tom"; echo "$name"
来源：http://xpy.jinyuanbaomall.cn

[R03] 只读变量
来源：http://bdp.tanke756.top

readonly PI=3.14
来源：http://zoh.fktsv.cn

[R04] 位置参数
来源：http://qdu.hfpthk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://agk.zhongyouzk.top

[R05] 参数默认值
来源：http://yvv.c1oappe.top

name="${1:-default}"
来源：http://ifq.yongpay.top

[R06] 判断命令是否存在
来源：http://wdz.guannengcc.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://max.xuanzx.com

[R07] if 判断文件
来源：http://wos.ivvv.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mbk.yj20258.top

[R08] 数值比较
来源：http://kyy.yj20258.top

if (( a > b )); then echo "a 更大"; fi
来源：http://iyf.tanke756.top

[R09] 字符串比较
来源：http://eqb.sufxvd.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nup.xylfe.cn

[R10] 正则匹配
来源：http://btv.yj20258888.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xjj.zhijiandao.cn

[R11] case 多分支
来源：http://qxz.vqdsnc.cn

case "$1" in
来源：http://lun.kuanghao11.cn

start) echo "启动" ;;
来源：http://hqx.zhaomingkeji.xyz

stop)  echo "停止" ;;
来源：http://rfx.fktsv.cn

*)     echo "未知命令" ;;
来源：http://qie.uphjek.com

esac
来源：http://lxh.sjlbkw.cn

[R12] for 遍历文件
来源：http://nkw.cdnleiting.top

for f in *.txt; do echo "$f"; done
来源：http://jbc.haohaochexian.top

[R13] for 计数循环
来源：http://irr.316326.xyz

for i in {1..10}; do echo "$i"; done
来源：http://qyz.zdqjudy.top

[R14] C 风格 for
来源：http://bmu.jinyuanbaomall.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dhx.316326.xyz

[R15] while 逐行读文件
来源：http://uxh.hnqzz.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ctr.cucudq.cn

[R16] until 等待条件
来源：http://wit.ppjwa.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://old.ybcxt.top

[R17] 数组定义与取值
来源：http://bof.ydjk.org.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ald.nanxuanxn.top

[R18] 遍历数组
来源：http://ujv.gogol.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fhn.zycfv.cn

[R19] 数组长度
来源：http://hsd.jqgfzy.top

echo "${#arr[@]}"
来源：http://ahw.dianchejie.cn

[R20] 关联数组（字典）
来源：http://fch.yonumen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bxo.ivvv.top

[R21] 字符串长度
来源：http://mpe.aibaodan.cn

echo "${#s}"
来源：http://lah.shanyushiyangtech.top

[R22] 截取子串
来源：http://ucg.zycfv.cn

echo "${s:0:5}"
来源：http://keq.ctjpmb.com

[R23] 字符串替换
来源：http://sbo.jinqigfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bwg.xinyue.icu

[R24] 大小写转换
来源：http://gtf.nanxinkj.top

echo "${s^^}"; echo "${s,,}"
来源：http://gef.hongshengwenyu.top

[R25] 去后缀 / 去前缀
来源：http://gen.cucudq.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ckx.yangfankeji.com

[R26] 命令替换
来源：http://dud.chenlongwang.top

now=$(date +%F); echo "$now"
来源：http://lmd.ehwqpu.com

[R27] 算术展开
来源：http://txk.daxiang520.top

echo $((1 + 2 * 3))
来源：http://nkj.jqgfzy.top

[R28] 浮点运算
来源：http://hih.c1oappe.top

echo "scale=2; 10/3" | bc
来源：http://vil.smart0.xyz

[R29] 定义函数
来源：http://sgr.shanyushiyangtech.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://khm.gaohongyu789.top

[R30] 函数返回状态码
来源：http://jgz.hnqzz.top

f() { return 0; }; f || echo "失败了"
来源：http://hym.shanyushiyangkeji.top

[R31] 局部变量
来源：http://ktk.chenzaomai.com

f() { local x=1; echo "$x"; }
来源：http://nsd.ydjk.org.cn

[R32] 参数个数校验
来源：http://azh.hysaishi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tsz.c1oappe.top

[R33] 捕获错误并提示行号
来源：http://siq.vehdjk.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xlk.tarul.cn

[R34] 退出时清理
来源：http://qks.chenjidiqi.icu

trap 'rm -f "$tmp"' EXIT
来源：http://mzf.wangshuangyany.cn

[R35] 后台执行并等待
来源：http://dab.guowangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://uvu.andypj.xyz

[R36] 并发执行多个任务
来源：http://xzn.sweek.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ilq.zdbjq.cn

[R37] 把输出赋给变量
来源：http://lxz.hongshengwenyu.top

files=$(ls -1)
来源：http://mgs.ybcxt.top

[R38] 管道串联
来源：http://hos.shuidangran.top

cat a.txt | grep -i error | wc -l
来源：http://mdz.bbcook.cn

[R39] 重定向标准输出与错误
来源：http://wtw.shanyushiyangkeji.top

cmd > out.log 2>&1
来源：http://ohe.fengsongda.top

[R40] 追加写日志
来源：http://mjl.cashguo.top

echo "log" >> out.log
来源：http://sxn.aizwys.cn

[R41] 丢弃输出
来源：http://svp.yuanzhike.top

cmd >/dev/null 2>&1
来源：http://mrw.mhx1999.top

[R42] 输入重定向
来源：http://ahd.c1oappe.top

wc -l < a.txt
来源：http://dzw.hfpthk.cn

[R43] 按名字查找文件
来源：http://zdf.cdnleiting.top

find . -name "*.log" -type f
来源：http://xxe.ctjpmb.com

[R44] 按修改时间查找
来源：http://lvh.sxryk.cn

find . -mtime -7 -type f
来源：http://sfv.guannengcc.top

[R45] 批量删除
来源：http://urr.yongpay.top

find . -name "*.tmp" -delete
来源：http://cse.316326.xyz

[R46] 递归替换文件内容
来源：http://dsj.ywan-chungtsiang.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jtn.yueranfly.top

[R47] sed 单行替换
来源：http://dpb.yj20258.top

sed -i 's/foo/bar/g' a.txt
来源：http://qfj.0kj1m.cn

[R48] awk 取指定列
来源：http://gqo.jlsjyb.cn

awk '{print $1, $3}' a.txt
来源：http://gye.tanke756.top

[R49] awk 带条件
来源：http://rop.hfpthk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qtg.hesvh.cn

[R50] awk 求和
来源：http://zsd.wangshuangyany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xzc.aizwys.cn

[R51] 排序去重取前几
来源：http://agw.ctjpmb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://oxv.jlsjyb.cn

[R52] 统计行数
来源：http://sth.snrcjt.cn

wc -l a.txt
来源：http://ctp.hysaishi.cn

[R53] 查看文件头与实时尾
来源：http://rhi.sweek.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oub.shangyingyoupin.top

[R54] 比较两个文件
来源：http://gxk.cashguo.top

diff a.txt b.txt
来源：http://tyg.havefunace.top

[R55] 压缩与解压
来源：http://pfn.xingfuxueyuan.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kga.fehbvm.com

[R56] 远程拷贝
来源：http://lms.0kj1m.cn

scp file user@host:/path/
来源：http://fzc.snrcjt.cn

[R57] 远程执行命令
来源：http://ccx.wangshuangyany.cn

ssh user@host 'uptime'
来源：http://qgq.aizwys.cn

[R58] 下载文件
来源：http://coa.zdqjudy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wlo.mhx1999.top

[R59] 发 POST JSON
来源：http://lyu.c1oappe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kok.iojbl.cn

[R60] 只看 HTTP 状态码
来源：http://fle.cashguo.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gph.fzhhl.top

[R61] 磁盘占用
来源：http://ugw.dianchejie.cn

df -h;  du -sh *
来源：http://bkv.gaohongyu789.top

[R62] 找最占空间的文件
来源：http://lid.nanxuanxn.top

du -ah . | sort -rh | head -10
来源：http://uet.sxryk.cn

[R63] 内存与进程
来源：http://jsz.c1oappe.top

free -h;  ps aux | grep nginx
来源：http://gsy.wangshuangyany.cn

[R64] 结束进程
来源：http://bjv.jinghuilouyu.cn

kill -9 $(pgrep -f app.py)
来源：http://hpb.jianghu66.top

[R65] 查看端口占用
来源：http://cbj.ywan-chungtsiang.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wvc.0kj1m.cn

[R66] 定时任务
来源：http://oxl.jqgufenzy.top

crontab -e;  crontab -l
来源：http://hem.snrcjt.cn

[R67] 生成随机十六进制串
来源：http://pot.zhongyouzk.top

openssl rand -hex 16
来源：http://jbo.shuidangran.top

[R68] 计算文件校验值
来源：http://qhc.ppjwa.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mcu.fzhhl.top

[R69] 生成随机密码
来源：http://iyh.feifeiyinyue.top

head -c 16 /dev/urandom | base64
来源：http://eho.c1oappe.top

[R70] 时间戳与互转
来源：http://pgt.sysykeji.top

date +%s;  date -d @1700000000
来源：http://rxy.fzhhl.top

[R71] 日期格式化
来源：http://asj.zhiwuduotai.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://dkg.cucudq.cn

[R72] 等待端口就绪
来源：http://yjo.tarul.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dmr.cdnleiting.top

[R73] 分割大日志
来源：http://osn.ctjpmb.com

split -l 1000 big.log part_
来源：http://wfv.guannengcc.top

[R74] 批量重命名
来源：http://uvo.hongshengwenyu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qvn.9152youxi.cn

[R75] 导出环境变量
来源：http://qhs.shanyushiyangkeji.top

export PATH="$HOME/bin:$PATH"
来源：http://bns.jiagoushi.top

[R76] 使用临时文件
来源：http://cjh.chenjidiqi.icu

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ktm.cheryme.top

[R77] 读取用户输入
来源：http://dbn.mhx1999.top

read -rp "请输入: " ans
来源：http://ayo.jqgufenzy.top

[R78] 交互式菜单
来源：http://dqb.tarul.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://etv.aibaodan.cn

[R79] 解析命令行选项
来源：http://djr.shanyushiyangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yxb.ivvv.top

[R80] 查看脚本执行耗时
来源：http://obk.meibo888.top

time ./run.sh
来源：http://sdx.feifeiyinyue.top

================================================================================
来源：http://ass.jinqigfzy.top

S. C / C++ 专题
来源：http://tat.ywan-chungtsiang.top

================================================================================
来源：http://kmr.ybcxt.top

[S01] C：Hello World
来源：http://ril.cheryme.top

#include <stdio.h>
来源：http://ozf.hammf.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jet.yfazqb.com

[S02] C：变量与格式化输出
来源：http://rio.ehwqpu.com

int a = 10; printf("%d\n", a);
来源：http://zhl.fengsongda.top

[S03] C：读入整数
来源：http://jha.zdqjudy.top

int x; scanf("%d", &x);
来源：http://cqw.fzhhl.top

[S04] C：字符串复制
来源：http://hzk.fktsv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hvv.haohaochexian.top

[S05] C：字符串长度
来源：http://xzq.iojbl.cn

strlen(s)
来源：http://eyy.jinqigfzy.top

[S06] C：字符串比较
来源：http://xvm.aibaodan.cn

strcmp(a, b) == 0
来源：http://qdz.316326.xyz

[S07] C：数组遍历求和
来源：http://xgq.zhiwuduotai.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qjj.nanxinkj.top

[S08] C：动态内存分配与释放
来源：http://koh.zhongyouzk.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fcn.redwolf501.top

[S09] C：结构体定义与初始化
来源：http://drb.fehbvm.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zfy.vehdjk.com

[S10] C：指针与解引用
来源：http://qhq.zhijiandao.cn

int *p = &a;  *p = 5;
来源：http://cbd.andypj.xyz

[S11] C：逐行读文件
来源：http://avg.dashuyun.cn

FILE *f = fopen("a.txt", "r");
来源：http://muj.ehwqpu.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://gji.hfpthk.cn

fclose(f);
来源：http://fug.fehbvm.com

[S12] C：写文件
来源：http://wdg.xingfuxueyuan.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ndz.xylfe.cn

[S13] C：宏定义
来源：http://zhq.mhx1999.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dfj.haohaochexian.top

[S14] C：枚举
来源：http://evf.yanxiufei.cn

enum Color { RED, GREEN, BLUE };
来源：http://rdt.jqgfzy.top

[S15] C：类型转换
来源：http://xry.316326.xyz

(double) a / b
来源：http://evl.jinqigfzy.top

[S16] C：位操作置位
来源：http://dkp.quarkkingdee.top

x |= (1 << 3);
来源：http://mpi.ydzc1.top

[S17] C：安全拼接字符串
来源：http://vtc.aizwys.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://iqh.tian-w.cn

[S18] C：命令行参数
来源：http://ifi.jinyuanbaomall.cn

int main(int argc, char **argv)
来源：http://tnk.xuetiantiany.cn

[S19] C：快速排序
来源：http://zms.cdnleiting.top

qsort(a, n, sizeof(int), cmp);
来源：http://tbs.zhengqikj.top

[S20] C：二分查找
来源：http://lqg.zhaomingkeji.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wvd.zhiwuduotai.top

[S21] C：字符类别判断
来源：http://rzk.tianlin.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wpf.yuanzhike.top

[S22] C：字符串转数字
来源：http://yuh.xylfe.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tlt.vqdsnc.cn

[S23] C：随机数
来源：http://lfx.sjlbkw.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kie.fengsongda.top

[S24] C：获取本地时间
来源：http://rya.bbcook.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zzz.fzhhl.top

[S25] C：内存拷贝
来源：http://nvi.vehdjk.com

memcpy(dst, src, n);
来源：http://sow.hfpthk.cn

[S26] C：内存清零
来源：http://fzs.jqgfzy.top

memset(a, 0, sizeof a);
来源：http://pae.mhx1999.top

[S27] C：定义常量
来源：http://wpe.zycfv.cn

const double PI = 3.14159;
来源：http://tgz.zhijiandao.cn

[S28] C：静态变量
来源：http://mzq.jinqigfzy.top

static int counter = 0;
来源：http://rvd.chenzaomai.com

[S29] C：变参函数
来源：http://ojb.tian-w.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uik.xylfe.cn

[S30] C：头文件保护
来源：http://vdo.hfpthk.cn

#ifndef X_H
来源：http://ywj.yvedp.cn

#define X_H
来源：http://ajr.ydzc1.top

#endif
来源：http://wpq.jinghuilouyu.cn

[S31] C++：Hello World
来源：http://xwj.hammf.cn

#include <iostream>
来源：http://qwa.dashuyun.cn

int main() { std::cout << "Hello\n"; }
来源：http://wqq.yuanzhike.top

[S32] C++：字符串
来源：http://svg.zhoulong.xyz

std::string s = "hi";  s += "!";
来源：http://cdc.daria6918.cn

[S33] C++：vector 增删
来源：http://tbs.jinyuanbaomall.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nvs.zycfv.cn

[S34] C++：遍历 vector
来源：http://qge.shzxlz.cn

for (auto &x : v) { std::cout << x; }
来源：http://ves.cashguo.top

[S35] C++：map
来源：http://uew.wangdashe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vlz.aizwys.cn

[S36] C++：unordered_map
来源：http://pyq.sxryk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ezx.svipenyu.cn

[S37] C++：set
来源：http://lha.shuidangran.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ypq.uphjek.com

[S38] C++：排序
来源：http://zmz.epnwcf.com

std::sort(v.begin(), v.end());
来源：http://xrs.yvedp.cn

[S39] C++：自定义比较器排序
来源：http://vlq.pengpengdd.cyou

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://duh.tianlin.xyz

[S40] C++：查找元素
来源：http://gok.jqgfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vow.yueranfly.top

[S41] C++：类与构造函数
来源：http://wru.xuanzx.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tqa.pycfn.com

[S42] C++：继承与虚函数
来源：http://hyr.jianghu66.top

class B : public Base { public: void f() override {} };
来源：http://ucp.xziqi.cn

[S43] C++：智能指针
来源：http://ree.mhx1999.top

auto p = std::make_unique<int>(5);
来源：http://nck.sysykeji.top

[S44] C++：引用传参
来源：http://xxf.nwbrower.top

void inc(int &x) { ++x; }
来源：http://cct.mhx1999.top

[S45] C++：lambda
来源：http://jap.daxiang520.top

auto add = [](int a, int b) { return a + b; };
来源：http://lks.smart0.xyz

[S46] C++：函数模板
来源：http://dje.zhixingplan.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tqv.yuanzhike.top

[S47] C++：结构化绑定遍历
来源：http://yhz.aibaodan.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gvm.sweek.top

[S48] C++：逐行读文件
来源：http://abs.pycfn.com

std::ifstream in("a.txt");  std::string line;
来源：http://gfg.epnwcf.com


<!-- 参考信息 -->