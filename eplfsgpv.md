代发 wailian999

[Q61] 移动平均
来源：http://nor.tian-w.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://eos.ivvv.top

[Q62] 分组占比
来源：http://lvb.andypj.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ibx.ehwqpu.com

[Q63] 开启事务
来源：http://eul.316326.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://aen.havefunace.top

[Q64] 提交事务
来源：http://pba.ydzc1.top

COMMIT;
来源：http://fxo.fanxiaobao.xyz

[Q65] 回滚事务
来源：http://qkv.hysaishi.cn

ROLLBACK;
来源：http://wfl.zhaomingkeji.xyz

[Q66] 行锁查询
来源：http://tuc.nanxinkj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nfq.fanxiaobao.xyz

[Q67] 设置隔离级别
来源：http://cmj.zdqjudy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://aka.jqgfzy.top

[Q68] 保存点
来源：http://sla.gogol.net.cn

SAVEPOINT sp1;
来源：http://kol.zdbjq.cn

ROLLBACK TO sp1;
来源：http://yga.hnxiangtu.top

[Q69] 查看执行计划
来源：http://wpy.shuidangran.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kzr.zycfv.cn

[Q70] 更新统计信息
来源：http://cpd.sufxvd.cn

ANALYZE TABLE users;
来源：http://wne.hesvh.cn

[Q71] 查看建表语句
来源：http://wyl.tarul.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hxw.mhx1999.top

[Q72] 查看索引
来源：http://sir.ydzc1.top

SHOW INDEX FROM users;
来源：http://enh.cashguo.top

[Q73] 查看表状态
来源：http://hbo.hfpthk.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zow.vehdjk.com

[Q74] 强制使用索引
来源：http://tjq.yvedp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bfr.hammf.cn

[Q75] 日期格式化
来源：http://xny.c1oappe.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://atp.sweek.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dda.vehdjk.com

[Q76] 按天统计
来源：http://gxj.svipenyu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rwt.cheryme.top

[Q77] 时间加减
来源：http://udj.hywenlv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://flp.xinyue.icu

[Q78] 当前时间
来源：http://pge.gotoacloud.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sqf.birdmap.top

[Q79] 字符串拼接
来源：http://jbf.redwolf501.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iph.wangshuangyany.cn

[Q80] 字符串截取
来源：http://pau.tarul.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tog.zhoulong.xyz

[Q81] 字符串替换
来源：http://vab.zhengqikj.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mbm.shuidangran.top

[Q82] 字符长度与字节长度
来源：http://jvq.xziqi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://brn.sjlbkw.cn

[Q83] 大小写转换
来源：http://zgw.jinqigfzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zab.cucudq.cn

[Q84] 去除首尾空格
来源：http://nru.kuanghao11.cn

SELECT TRIM(name) FROM users;
来源：http://vvo.andypj.xyz

[Q85] 数值取整
来源：http://ghd.tianlin.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uao.aibaodan.cn

[Q86] 读取 JSON 字段
来源：http://zcr.tanke756.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gfe.guowangkeji.top

[Q87] JSON 字段做条件
来源：http://mjz.vehdjk.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jfp.havefunace.top

[Q88] 行转列（条件聚合）
来源：http://dwp.fzhhl.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hsj.nwbrower.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zao.shzxlz.cn

[Q89] 判断表是否存在
来源：http://eqx.yvedp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hxu.jianghu66.top

[Q90] 生成序号列
来源：http://knk.xuetiantiany.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xxz.jinyuanbaomall.cn

================================================================================
来源：http://ujl.zhiwuduotai.top

R. Bash 专题
来源：http://kue.cheryme.top

================================================================================
来源：http://tbr.tian-w.cn

[R01] shebang 与严格模式
来源：http://ubm.jqgfzy.top

#!/usr/bin/env bash
来源：http://dtt.nanxinkj.top

set -euo pipefail
来源：http://yve.ehwqpu.com

[R02] 变量赋值与使用
来源：http://bov.yuanzhike.top

name="Tom"; echo "$name"
来源：http://vak.yueranfly.top

[R03] 只读变量
来源：http://myt.sweek.top

readonly PI=3.14
来源：http://scl.havefunace.top

[R04] 位置参数
来源：http://ibr.cdnleiting.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fzj.sjlbkw.cn

[R05] 参数默认值
来源：http://liz.ehwqpu.com

name="${1:-default}"
来源：http://zsm.zhiwuduotai.top

[R06] 判断命令是否存在
来源：http://gay.yuxming.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xmy.snrcjt.cn

[R07] if 判断文件
来源：http://rha.yuxming.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bob.xingfuxueyuan.xyz

[R08] 数值比较
来源：http://qdl.tanke756.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vgz.zdqjudy.top

[R09] 字符串比较
来源：http://izn.jiagoushi.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://axk.hnxiangtu.top

[R10] 正则匹配
来源：http://ihz.guannengcc.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://biu.cqqwz.cn

[R11] case 多分支
来源：http://gna.shanyushiyangkeji.top

case "$1" in
来源：http://nsv.bbcook.cn

start) echo "启动" ;;
来源：http://qna.fzhhl.top

stop)  echo "停止" ;;
来源：http://jav.havefunace.top

*)     echo "未知命令" ;;
来源：http://lwy.hongshengwenyu.top

esac
来源：http://hug.zhengqikj.top

[R12] for 遍历文件
来源：http://nxy.yueranfly.top

for f in *.txt; do echo "$f"; done
来源：http://ecn.yueranfly.top

[R13] for 计数循环
来源：http://ygn.chenzaomai.com

for i in {1..10}; do echo "$i"; done
来源：http://rjd.aibaodan.cn

[R14] C 风格 for
来源：http://hcy.yfazqb.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fub.daria6918.cn

[R15] while 逐行读文件
来源：http://vzq.zhijiandao.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lho.yuxming.cn

[R16] until 等待条件
来源：http://dgv.smart0.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gto.hnqzz.top

[R17] 数组定义与取值
来源：http://tpo.jiagoushi.top

arr=(a b c); echo "${arr[0]}"
来源：http://evb.xuetiantiany.cn

[R18] 遍历数组
来源：http://uvm.sweek.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ssi.sjlbkw.cn

[R19] 数组长度
来源：http://hgw.tian-w.cn

echo "${#arr[@]}"
来源：http://tgb.smart0.xyz

[R20] 关联数组（字典）
来源：http://dmd.vehdjk.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pkb.vqdsnc.cn

[R21] 字符串长度
来源：http://qhc.shuidangran.top

echo "${#s}"
来源：http://lto.dashuyun.cn

[R22] 截取子串
来源：http://zpj.fzhhl.top

echo "${s:0:5}"
来源：http://rgn.nanxuanxn.top

[R23] 字符串替换
来源：http://hjy.chenlongwang.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zpk.bjfxy.top

[R24] 大小写转换
来源：http://gvu.jlsjyb.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pho.dashuyun.cn

[R25] 去后缀 / 去前缀
来源：http://yji.fzhhl.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://xsg.xuetiantiany.cn

[R26] 命令替换
来源：http://zss.ppjwa.cn

now=$(date +%F); echo "$now"
来源：http://mpp.zhongyouzk.top

[R27] 算术展开
来源：http://ooy.shanyushiyangtech.top

echo $((1 + 2 * 3))
来源：http://ayo.yuanzhike.top

[R28] 浮点运算
来源：http://chv.gzhubu.top

echo "scale=2; 10/3" | bc
来源：http://sys.pycfn.com

[R29] 定义函数
来源：http://mxo.gogol.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pgg.wangdashe.top

[R30] 函数返回状态码
来源：http://tdf.birdmap.top

f() { return 0; }; f || echo "失败了"
来源：http://qei.ctjpmb.com

[R31] 局部变量
来源：http://hrw.yueranfly.top

f() { local x=1; echo "$x"; }
来源：http://eab.jinqigufen.top

[R32] 参数个数校验
来源：http://dsf.shzxlz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oyw.chenjidiqi.icu

[R33] 捕获错误并提示行号
来源：http://weo.xziqi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nyt.zhijiandao.cn

[R34] 退出时清理
来源：http://mkk.tian-w.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qej.guannengcc.top

[R35] 后台执行并等待
来源：http://xwi.vqdsnc.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gbj.hnqzz.top

[R36] 并发执行多个任务
来源：http://haj.shuidangran.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xsc.ctjpmb.com

[R37] 把输出赋给变量
来源：http://wxd.yuanzhike.top

files=$(ls -1)
来源：http://wqf.0kj1m.cn

[R38] 管道串联
来源：http://exb.nwbrower.top

cat a.txt | grep -i error | wc -l
来源：http://tug.zhijiandao.cn

[R39] 重定向标准输出与错误
来源：http://nxj.svipenyu.cn

cmd > out.log 2>&1
来源：http://pec.dianchejie.cn

[R40] 追加写日志
来源：http://qpv.ydjk.org.cn

echo "log" >> out.log
来源：http://lbn.jqgufenzy.top

[R41] 丢弃输出
来源：http://ldm.jqgfzy.top

cmd >/dev/null 2>&1
来源：http://buj.sweek.top

[R42] 输入重定向
来源：http://trv.yueranfly.top

wc -l < a.txt
来源：http://mdc.fengsongda.top

[R43] 按名字查找文件
来源：http://vbd.316326.xyz

find . -name "*.log" -type f
来源：http://tdd.quarkkingdee.top

[R44] 按修改时间查找
来源：http://pvh.sufxvd.cn

find . -mtime -7 -type f
来源：http://xhr.dianchejie.cn

[R45] 批量删除
来源：http://jlh.jinqigufen.top

find . -name "*.tmp" -delete
来源：http://wmi.shanyushiyangkeji.top

[R46] 递归替换文件内容
来源：http://aat.vqdsnc.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yzm.vehdjk.com

[R47] sed 单行替换
来源：http://yed.yj20258888.top

sed -i 's/foo/bar/g' a.txt
来源：http://gjc.epnwcf.com

[R48] awk 取指定列
来源：http://afz.sweek.top

awk '{print $1, $3}' a.txt
来源：http://nzk.zhoulong.xyz

[R49] awk 带条件
来源：http://ldw.yfazqb.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tjp.haohaochexian.top

[R50] awk 求和
来源：http://iie.vehdjk.com

awk '{s += $2} END {print s}' a.txt
来源：http://unp.wangshuangyany.cn

[R51] 排序去重取前几
来源：http://htq.zhoulong.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://wib.0kj1m.cn

[R52] 统计行数
来源：http://zra.tanke756.top

wc -l a.txt
来源：http://vpj.chenlongwang.top

[R53] 查看文件头与实时尾
来源：http://sdp.fanxiaobao.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lkx.svipenyu.cn

[R54] 比较两个文件
来源：http://tga.bjfxy.top

diff a.txt b.txt
来源：http://cul.shanyushiyangtech.top

[R55] 压缩与解压
来源：http://aii.cdnleiting.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://muz.guannengcc.top

[R56] 远程拷贝
来源：http://vfh.hammf.cn

scp file user@host:/path/
来源：http://dmy.yj20258888.top

[R57] 远程执行命令
来源：http://qwu.shanyushiyangtech.top

ssh user@host 'uptime'
来源：http://akf.yanxiufei.cn

[R58] 下载文件
来源：http://kka.cdnleiting.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://crl.fehbvm.com

[R59] 发 POST JSON
来源：http://hqk.wangshuangyany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cke.xuanzx.com

[R60] 只看 HTTP 状态码
来源：http://nfs.xylfe.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://spu.nanxuanxn.top

[R61] 磁盘占用
来源：http://wjd.jqgfzy.top

df -h;  du -sh *
来源：http://let.sjlbkw.cn

[R62] 找最占空间的文件
来源：http://zcp.birdmap.top

du -ah . | sort -rh | head -10
来源：http://cph.aibaodan.cn

[R63] 内存与进程
来源：http://bxt.zdqjudy.top

free -h;  ps aux | grep nginx
来源：http://fpw.ybcxt.top

[R64] 结束进程
来源：http://tmf.bbcook.cn

kill -9 $(pgrep -f app.py)
来源：http://paf.316326.xyz

[R65] 查看端口占用
来源：http://sma.cheryme.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qmo.ydjk.org.cn

[R66] 定时任务
来源：http://muk.ehwqpu.com

crontab -e;  crontab -l
来源：http://plt.zhijiandao.cn

[R67] 生成随机十六进制串
来源：http://nya.yonumen.top

openssl rand -hex 16
来源：http://vop.jyoumei.cn

[R68] 计算文件校验值
来源：http://ycm.hysaishi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://enl.fanxiaobao.xyz

[R69] 生成随机密码
来源：http://kcw.wangdashe.top

head -c 16 /dev/urandom | base64
来源：http://yfi.fanxiaobao.xyz

[R70] 时间戳与互转
来源：http://laq.pycfn.com

date +%s;  date -d @1700000000
来源：http://iko.cashguo.top

[R71] 日期格式化
来源：http://qai.gotoacloud.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qib.316326.xyz

[R72] 等待端口就绪
来源：http://wbw.uphjek.com

until nc -z localhost 3306; do sleep 1; done
来源：http://iku.tarul.cn

[R73] 分割大日志
来源：http://cvt.pycfn.com

split -l 1000 big.log part_
来源：http://ihr.guannengcc.top

[R74] 批量重命名
来源：http://uja.xingfuxueyuan.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cfj.shangyingyoupin.top

[R75] 导出环境变量
来源：http://tmt.hysaishi.cn

export PATH="$HOME/bin:$PATH"
来源：http://gxf.tian-w.cn

[R76] 使用临时文件
来源：http://ceo.ydjk.org.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hkp.jqgufenzy.top

[R77] 读取用户输入
来源：http://khm.hesvh.cn

read -rp "请输入: " ans
来源：http://gwf.zhongyouzk.top

[R78] 交互式菜单
来源：http://nbs.ctjpmb.com

select opt in a b c; do echo "$opt"; break; done
来源：http://hky.jqgufenzy.top

[R79] 解析命令行选项
来源：http://wrd.9152youxi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ntn.svipenyu.cn

[R80] 查看脚本执行耗时
来源：http://aas.xylfe.cn

time ./run.sh
来源：http://udz.xinyue.icu

================================================================================
来源：http://rzh.kuanghao11.cn

S. C / C++ 专题
来源：http://qgb.ivvv.top

================================================================================
来源：http://zpi.shuidangran.top

[S01] C：Hello World
来源：http://vqg.dianchejie.cn

#include <stdio.h>
来源：http://nnx.yfazqb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://eqq.yj20258.top

[S02] C：变量与格式化输出
来源：http://pbh.ivvv.top

int a = 10; printf("%d\n", a);
来源：http://ppw.nanxuanxn.top

[S03] C：读入整数
来源：http://xni.yj20258.top

int x; scanf("%d", &x);
来源：http://rfh.tanke756.top

[S04] C：字符串复制
来源：http://afr.fktsv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nzv.sufxvd.cn

[S05] C：字符串长度
来源：http://hgu.bbcook.cn

strlen(s)
来源：http://dqa.gzhubu.top

[S06] C：字符串比较
来源：http://fbv.ydjk.org.cn

strcmp(a, b) == 0
来源：http://sii.yj20258.top

[S07] C：数组遍历求和
来源：http://clt.aibaodan.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mrr.hfpthk.cn

[S08] C：动态内存分配与释放
来源：http://udl.fzhhl.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lmf.gaohongyu789.top

[S09] C：结构体定义与初始化
来源：http://oqn.cashguo.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yoq.fanxiaobao.xyz

[S10] C：指针与解引用
来源：http://mhj.shzxlz.cn

int *p = &a;  *p = 5;
来源：http://cfz.andypj.xyz

[S11] C：逐行读文件
来源：http://vdi.aizwys.cn

FILE *f = fopen("a.txt", "r");
来源：http://gfp.redwolf501.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ecl.ydjk.org.cn

fclose(f);
来源：http://toy.gogol.net.cn

[S12] C：写文件
来源：http://pij.bbcook.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xty.yuanzhike.top

[S13] C：宏定义
来源：http://ono.ybcxt.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rjy.xziqi.cn

[S14] C：枚举
来源：http://ccf.birdmap.top

enum Color { RED, GREEN, BLUE };
来源：http://vsm.ctjpmb.com

[S15] C：类型转换
来源：http://qcl.jyoumei.cn

(double) a / b
来源：http://mmz.jqgufenzy.top

[S16] C：位操作置位
来源：http://tjs.sysykeji.top

x |= (1 << 3);
来源：http://ewo.daxiang520.top

[S17] C：安全拼接字符串
来源：http://mcn.havefunace.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kye.fanxiaobao.xyz

[S18] C：命令行参数
来源：http://hrg.yuanzhike.top

int main(int argc, char **argv)
来源：http://wqf.xziqi.cn

[S19] C：快速排序
来源：http://rwc.sweek.top

qsort(a, n, sizeof(int), cmp);
来源：http://wpo.fzhhl.top

[S20] C：二分查找
来源：http://eav.gogol.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jvl.xingfuxueyuan.xyz

[S21] C：字符类别判断
来源：http://tjw.shangyingyoupin.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uxk.bbcook.cn

[S22] C：字符串转数字
来源：http://aiu.aibaodan.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gzc.bbcook.cn

[S23] C：随机数
来源：http://fka.vehdjk.com

srand(time(NULL));  int r = rand() % 100;
来源：http://qqk.zhaomingkeji.xyz

[S24] C：获取本地时间
来源：http://bej.svipenyu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ddt.zdbjq.cn

[S25] C：内存拷贝
来源：http://hve.sxryk.cn

memcpy(dst, src, n);
来源：http://jky.zhongyouzk.top

[S26] C：内存清零
来源：http://jhc.sysykeji.top

memset(a, 0, sizeof a);
来源：http://hhz.yuxming.cn

[S27] C：定义常量
来源：http://oxx.yongpay.top

const double PI = 3.14159;
来源：http://qmm.meibo888.top

[S28] C：静态变量
来源：http://lrd.guowangkeji.top

static int counter = 0;
来源：http://vvd.sweek.top

[S29] C：变参函数
来源：http://mzd.iojbl.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wqs.yonumen.top

[S30] C：头文件保护
来源：http://tdw.jiagoushi.top

#ifndef X_H
来源：http://baz.yj20258.top

#define X_H
来源：http://mxi.ywan-chungtsiang.top

#endif
来源：http://zze.bbcook.cn

[S31] C++：Hello World
来源：http://chq.hcnkem.com


<!-- 参考信息 -->