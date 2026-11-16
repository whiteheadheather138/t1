代发 wailian999

[Q78] 当前时间
来源：http://adh.cdnleiting.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hqo.dashuyun.cn

[Q79] 字符串拼接
来源：http://toa.vqdsnc.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ruv.hongshengwenyu.top

[Q80] 字符串截取
来源：http://pky.bjfxy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jpt.shuidangran.top

[Q81] 字符串替换
来源：http://znq.havefunace.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fvm.ydjk.org.cn

[Q82] 字符长度与字节长度
来源：http://gzq.iojbl.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pig.quarkkingdee.top

[Q83] 大小写转换
来源：http://nmk.meibo888.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://iff.vehdjk.com

[Q84] 去除首尾空格
来源：http://wsv.hongshengwenyu.top

SELECT TRIM(name) FROM users;
来源：http://prr.tarul.cn

[Q85] 数值取整
来源：http://fqw.chenjidiqi.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qdb.ppjwa.cn

[Q86] 读取 JSON 字段
来源：http://rth.quarkkingdee.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hut.gotoacloud.top

[Q87] JSON 字段做条件
来源：http://igb.epnwcf.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oav.xziqi.cn

[Q88] 行转列（条件聚合）
来源：http://vpn.xinyue.icu

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qim.jinqigufen.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ggt.ybcxt.top

[Q89] 判断表是否存在
来源：http://sjy.iojbl.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ggn.hcnkem.com

[Q90] 生成序号列
来源：http://ttu.fehbvm.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://iuk.birdmap.top

================================================================================
来源：http://qkb.xylfe.cn

R. Bash 专题
来源：http://yoj.yonumen.top

================================================================================
来源：http://mse.iojbl.cn

[R01] shebang 与严格模式
来源：http://fdc.gogol.net.cn

#!/usr/bin/env bash
来源：http://fzk.redwolf501.top

set -euo pipefail
来源：http://rpd.jiagoushi.top

[R02] 变量赋值与使用
来源：http://adw.c1oappe.top

name="Tom"; echo "$name"
来源：http://rez.guannengcc.top

[R03] 只读变量
来源：http://xyk.yanxiufei.cn

readonly PI=3.14
来源：http://bau.jiagoushi.top

[R04] 位置参数
来源：http://zyl.nanxuanxn.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ohr.gogol.net.cn

[R05] 参数默认值
来源：http://fav.birdmap.top

name="${1:-default}"
来源：http://quu.gaohongyu789.top

[R06] 判断命令是否存在
来源：http://ixl.fzhhl.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jgu.nanxuanxn.top

[R07] if 判断文件
来源：http://ogk.hammf.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rkl.jinqigfzy.top

[R08] 数值比较
来源：http://fgs.yfazqb.com

if (( a > b )); then echo "a 更大"; fi
来源：http://bgd.daria6918.cn

[R09] 字符串比较
来源：http://bib.jqgfzy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nvo.guowangkeji.top

[R10] 正则匹配
来源：http://crq.fzhhl.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qxd.vqdsnc.cn

[R11] case 多分支
来源：http://yvp.jyoumei.cn

case "$1" in
来源：http://vmj.shuidangran.top

start) echo "启动" ;;
来源：http://rvu.tanke756.top

stop)  echo "停止" ;;
来源：http://aqq.jinyuanbaomall.cn

*)     echo "未知命令" ;;
来源：http://ncy.zhiwuduotai.top

esac
来源：http://lbe.ybcxt.top

[R12] for 遍历文件
来源：http://gbc.zycfv.cn

for f in *.txt; do echo "$f"; done
来源：http://spi.jinghuilouyu.cn

[R13] for 计数循环
来源：http://vol.nanxuanxn.top

for i in {1..10}; do echo "$i"; done
来源：http://wsz.zdqjudy.top

[R14] C 风格 for
来源：http://iuw.sxryk.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ohw.tianlin.xyz

[R15] while 逐行读文件
来源：http://dgp.daxiang520.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nwz.gogol.net.cn

[R16] until 等待条件
来源：http://cln.jqgufenzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ltj.yvedp.cn

[R17] 数组定义与取值
来源：http://dqr.ywan-chungtsiang.top

arr=(a b c); echo "${arr[0]}"
来源：http://lrk.hysaishi.cn

[R18] 遍历数组
来源：http://rdr.redwolf501.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rig.gogol.net.cn

[R19] 数组长度
来源：http://hkc.chenjidiqi.icu

echo "${#arr[@]}"
来源：http://fdr.pengpengdd.cyou

[R20] 关联数组（字典）
来源：http://ven.jinyuanbaomall.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hfz.snrcjt.cn

[R21] 字符串长度
来源：http://osv.tian-w.cn

echo "${#s}"
来源：http://rqr.wangshuangyany.cn

[R22] 截取子串
来源：http://wzf.sysykeji.top

echo "${s:0:5}"
来源：http://vvp.ywan-chungtsiang.top

[R23] 字符串替换
来源：http://msn.chenjidiqi.icu

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tsk.wangdashe.top

[R24] 大小写转换
来源：http://aqk.ivvv.top

echo "${s^^}"; echo "${s,,}"
来源：http://giz.shanyushiyangkeji.top

[R25] 去后缀 / 去前缀
来源：http://eoo.pengpengdd.cyou

echo "${f%.txt}"; echo "${f#./}"
来源：http://bmi.zhoulong.xyz

[R26] 命令替换
来源：http://dfs.jinqigfzy.top

now=$(date +%F); echo "$now"
来源：http://xuq.hywenlv.cn

[R27] 算术展开
来源：http://opm.hcnkem.com

echo $((1 + 2 * 3))
来源：http://dtd.hesvh.cn

[R28] 浮点运算
来源：http://xrx.xuetiantiany.cn

echo "scale=2; 10/3" | bc
来源：http://ydz.sysykeji.top

[R29] 定义函数
来源：http://shk.havefunace.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cdd.tian-w.cn

[R30] 函数返回状态码
来源：http://tkb.andypj.xyz

f() { return 0; }; f || echo "失败了"
来源：http://jbv.sweek.top

[R31] 局部变量
来源：http://vkz.gotoacloud.top

f() { local x=1; echo "$x"; }
来源：http://qic.ppjwa.cn

[R32] 参数个数校验
来源：http://tfr.wangdashe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dkp.aibaodan.cn

[R33] 捕获错误并提示行号
来源：http://jqx.hongshengwenyu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://emd.pengpengdd.cyou

[R34] 退出时清理
来源：http://onn.hfpthk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ewg.gaohongyu789.top

[R35] 后台执行并等待
来源：http://aam.tian-w.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://usi.fengsongda.top

[R36] 并发执行多个任务
来源：http://vtn.shanyushiyangtech.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bvk.tanke756.top

[R37] 把输出赋给变量
来源：http://ilc.tianlin.xyz

files=$(ls -1)
来源：http://nvj.yongpay.top

[R38] 管道串联
来源：http://xqs.sysykeji.top

cat a.txt | grep -i error | wc -l
来源：http://nen.9152youxi.cn

[R39] 重定向标准输出与错误
来源：http://foa.jqgufenzy.top

cmd > out.log 2>&1
来源：http://cei.316326.xyz

[R40] 追加写日志
来源：http://bzg.iojbl.cn

echo "log" >> out.log
来源：http://xof.pengpengdd.cyou

[R41] 丢弃输出
来源：http://ulk.daria6918.cn

cmd >/dev/null 2>&1
来源：http://xgy.yj202588.top

[R42] 输入重定向
来源：http://org.shanyushiyangtech.top

wc -l < a.txt
来源：http://mbr.wangdashe.top

[R43] 按名字查找文件
来源：http://iza.ctjpmb.com

find . -name "*.log" -type f
来源：http://zhs.hcnkem.com

[R44] 按修改时间查找
来源：http://cwg.yueranfly.top

find . -mtime -7 -type f
来源：http://vmp.zhiwuduotai.top

[R45] 批量删除
来源：http://die.yfazqb.com

find . -name "*.tmp" -delete
来源：http://isi.aibaodan.cn

[R46] 递归替换文件内容
来源：http://yag.yj202588.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sor.fzhhl.top

[R47] sed 单行替换
来源：http://hxf.yueranfly.top

sed -i 's/foo/bar/g' a.txt
来源：http://qgt.feifeiyinyue.top

[R48] awk 取指定列
来源：http://poj.andypj.xyz

awk '{print $1, $3}' a.txt
来源：http://txw.yj202588.top

[R49] awk 带条件
来源：http://rle.gaohongyu789.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dsd.jianghu66.top

[R50] awk 求和
来源：http://opp.yuanzhike.top

awk '{s += $2} END {print s}' a.txt
来源：http://ekc.cucudq.cn

[R51] 排序去重取前几
来源：http://bii.andypj.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://yex.yj20258.top

[R52] 统计行数
来源：http://vax.zhengqikj.top

wc -l a.txt
来源：http://ooc.shanyushiyangtech.top

[R53] 查看文件头与实时尾
来源：http://xya.sweek.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kgs.fzhhl.top

[R54] 比较两个文件
来源：http://eak.ivvv.top

diff a.txt b.txt
来源：http://zfs.nanxinkj.top

[R55] 压缩与解压
来源：http://kzw.316326.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gcv.svipenyu.cn

[R56] 远程拷贝
来源：http://vnr.zhengqikj.top

scp file user@host:/path/
来源：http://uqd.zhongyouzk.top

[R57] 远程执行命令
来源：http://ecu.fktsv.cn

ssh user@host 'uptime'
来源：http://erf.yangfankeji.com

[R58] 下载文件
来源：http://rdy.guowangkeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sna.jlsjyb.cn

[R59] 发 POST JSON
来源：http://xml.cheryme.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kix.fanxiaobao.xyz

[R60] 只看 HTTP 状态码
来源：http://mei.meibo888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://shw.epnwcf.com

[R61] 磁盘占用
来源：http://eaz.jinghuilouyu.cn

df -h;  du -sh *
来源：http://alw.daria6918.cn

[R62] 找最占空间的文件
来源：http://hfz.cashguo.top

du -ah . | sort -rh | head -10
来源：http://hiv.jinyuanbaomall.cn

[R63] 内存与进程
来源：http://cde.daxiang520.top

free -h;  ps aux | grep nginx
来源：http://jlg.chenjidiqi.icu

[R64] 结束进程
来源：http://eri.yvedp.cn

kill -9 $(pgrep -f app.py)
来源：http://iql.0kj1m.cn

[R65] 查看端口占用
来源：http://wvq.yueranfly.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kog.feifeiyinyue.top

[R66] 定时任务
来源：http://yqu.meibo888.top

crontab -e;  crontab -l
来源：http://jei.cheryme.top

[R67] 生成随机十六进制串
来源：http://wdi.cdnleiting.top

openssl rand -hex 16
来源：http://fjn.hcnkem.com

[R68] 计算文件校验值
来源：http://nxv.snrcjt.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nnk.tianlin.xyz

[R69] 生成随机密码
来源：http://fla.gogol.net.cn

head -c 16 /dev/urandom | base64
来源：http://luz.yj20258888.top

[R70] 时间戳与互转
来源：http://xho.xylfe.cn

date +%s;  date -d @1700000000
来源：http://pom.yuxming.cn

[R71] 日期格式化
来源：http://uys.yj202588.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://dhx.xuanzx.com

[R72] 等待端口就绪
来源：http://eec.cucudq.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://amp.xingfuxueyuan.xyz

[R73] 分割大日志
来源：http://bce.hesvh.cn

split -l 1000 big.log part_
来源：http://zgd.zhaomingkeji.xyz

[R74] 批量重命名
来源：http://fgf.yvedp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kfv.xylfe.cn

[R75] 导出环境变量
来源：http://guw.nanxinkj.top

export PATH="$HOME/bin:$PATH"
来源：http://hbt.iojbl.cn

[R76] 使用临时文件
来源：http://pbi.fanxiaobao.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ohq.gzhubu.top

[R77] 读取用户输入
来源：http://kvg.xinyue.icu

read -rp "请输入: " ans
来源：http://gap.snrcjt.cn

[R78] 交互式菜单
来源：http://ysm.jqgufenzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://bim.shangyingyoupin.top

[R79] 解析命令行选项
来源：http://xgn.hesvh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oii.chenjidiqi.icu

[R80] 查看脚本执行耗时
来源：http://qcc.chenzaomai.com

time ./run.sh
来源：http://wze.quarkkingdee.top

================================================================================
来源：http://uxz.epnwcf.com

S. C / C++ 专题
来源：http://mun.sxryk.cn

================================================================================
来源：http://nmh.fengsongda.top

[S01] C：Hello World
来源：http://dhl.yj20258.top

#include <stdio.h>
来源：http://ppb.cqqwz.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cwq.sxryk.cn

[S02] C：变量与格式化输出
来源：http://vzr.xuetiantiany.cn

int a = 10; printf("%d\n", a);
来源：http://cqp.nwbrower.top

[S03] C：读入整数
来源：http://jee.feifeiyinyue.top

int x; scanf("%d", &x);
来源：http://wvk.tian-w.cn

[S04] C：字符串复制
来源：http://iax.tanke756.top

char dst[32]; strcpy(dst, "hi");
来源：http://wls.meibo888.top

[S05] C：字符串长度
来源：http://dmy.bjfxy.top

strlen(s)
来源：http://xgk.xuetiantiany.cn

[S06] C：字符串比较
来源：http://jpf.hywenlv.cn

strcmp(a, b) == 0
来源：http://wcw.sjlbkw.cn

[S07] C：数组遍历求和
来源：http://wcv.tianlin.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rer.hnqzz.top

[S08] C：动态内存分配与释放
来源：http://cdz.shuidangran.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://txg.svipenyu.cn

[S09] C：结构体定义与初始化
来源：http://gmr.feifeiyinyue.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jct.andypj.xyz

[S10] C：指针与解引用
来源：http://nyw.kuanghao11.cn

int *p = &a;  *p = 5;
来源：http://znd.zhengqikj.top

[S11] C：逐行读文件
来源：http://cro.cashguo.top

FILE *f = fopen("a.txt", "r");
来源：http://xxi.52xcode.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pqp.zhijiandao.cn

fclose(f);
来源：http://xov.sufxvd.cn

[S12] C：写文件
来源：http://vtl.zhongyouzk.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fcw.sxryk.cn

[S13] C：宏定义
来源：http://ovu.yfazqb.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vfr.yanxiufei.cn

[S14] C：枚举
来源：http://mfv.hnqzz.top

enum Color { RED, GREEN, BLUE };
来源：http://oyk.wangdashe.top

[S15] C：类型转换
来源：http://wou.hcnkem.com

(double) a / b
来源：http://azq.jinyuanbaomall.cn

[S16] C：位操作置位
来源：http://bsd.hcnkem.com

x |= (1 << 3);
来源：http://ety.birdmap.top

[S17] C：安全拼接字符串
来源：http://mct.bbcook.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bbz.feifeiyinyue.top

[S18] C：命令行参数
来源：http://xxj.hcnkem.com

int main(int argc, char **argv)
来源：http://quj.hnqzz.top

[S19] C：快速排序
来源：http://jgu.yanxiufei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tif.xuetiantiany.cn

[S20] C：二分查找
来源：http://eyj.zhiwuduotai.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oyt.sysykeji.top

[S21] C：字符类别判断
来源：http://xci.shuidangran.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qdw.sxryk.cn

[S22] C：字符串转数字
来源：http://lda.ctjpmb.com

atoi("42");  strtod("3.14", NULL);
来源：http://ope.9152youxi.cn

[S23] C：随机数
来源：http://miw.hnqzz.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xye.fehbvm.com

[S24] C：获取本地时间
来源：http://bmi.sxryk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hjk.jinqigfzy.top

[S25] C：内存拷贝
来源：http://aui.daria6918.cn

memcpy(dst, src, n);
来源：http://qiy.sufxvd.cn

[S26] C：内存清零
来源：http://znh.svipenyu.cn

memset(a, 0, sizeof a);
来源：http://izu.yvedp.cn

[S27] C：定义常量
来源：http://uri.nanxuanxn.top

const double PI = 3.14159;
来源：http://phq.havefunace.top

[S28] C：静态变量
来源：http://wup.shangyingyoupin.top

static int counter = 0;
来源：http://eel.ywan-chungtsiang.top

[S29] C：变参函数
来源：http://hxi.fengsongda.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ahv.epnwcf.com

[S30] C：头文件保护
来源：http://umq.c1oappe.top

#ifndef X_H
来源：http://rke.ywan-chungtsiang.top

#define X_H
来源：http://yof.ivvv.top

#endif
来源：http://jhs.shzxlz.cn

[S31] C++：Hello World
来源：http://mls.zhongyouzk.top

#include <iostream>
来源：http://fbo.uphjek.com

int main() { std::cout << "Hello\n"; }
来源：http://ajq.hesvh.cn

[S32] C++：字符串
来源：http://qcp.yvedp.cn

std::string s = "hi";  s += "!";
来源：http://dvu.gaohongyu789.top

[S33] C++：vector 增删
来源：http://aoi.kuanghao11.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ndy.yuanzhike.top

[S34] C++：遍历 vector
来源：http://dnz.snrcjt.cn

for (auto &x : v) { std::cout << x; }
来源：http://hme.sxryk.cn

[S35] C++：map
来源：http://bej.hnxiangtu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://srg.yj20258888.top

[S36] C++：unordered_map
来源：http://jxh.pengpengdd.cyou

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bwv.dashuyun.cn

[S37] C++：set
来源：http://sqw.zhengqikj.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://znn.ydjk.org.cn

[S38] C++：排序
来源：http://job.ybcxt.top

std::sort(v.begin(), v.end());
来源：http://cxr.sufxvd.cn

[S39] C++：自定义比较器排序
来源：http://waz.xziqi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://thx.uphjek.com

[S40] C++：查找元素
来源：http://uqz.cdnleiting.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uig.xinyue.icu

[S41] C++：类与构造函数
来源：http://smz.hnxiangtu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zfv.ppjwa.cn

[S42] C++：继承与虚函数
来源：http://svy.mhx1999.top

class B : public Base { public: void f() override {} };
来源：http://bpi.yj20258888.top

[S43] C++：智能指针
来源：http://yyp.nwbrower.top

auto p = std::make_unique<int>(5);
来源：http://qag.nanxuanxn.top

[S44] C++：引用传参
来源：http://zzv.jqgufenzy.top

void inc(int &x) { ++x; }
来源：http://jxl.nanxuanxn.top

[S45] C++：lambda
来源：http://nfi.ydjk.org.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qic.snrcjt.cn

[S46] C++：函数模板
来源：http://hpe.shanyushiyangkeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vhl.nwbrower.top

[S47] C++：结构化绑定遍历
来源：http://ufa.redwolf501.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xcs.jianghu66.top

[S48] C++：逐行读文件
来源：http://vxz.ppjwa.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zda.hammf.cn


<!-- 参考信息 -->