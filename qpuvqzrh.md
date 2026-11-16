代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tkg.tanke756.top

[Q60] 取上一行 / 下一行
来源：http://uxh.daria6918.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fop.zhongyouzk.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gtd.hywenlv.cn

[Q61] 移动平均
来源：http://esj.ydjk.org.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://aic.jlsjyb.cn

[Q62] 分组占比
来源：http://tan.sweek.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://efn.wangshuangyany.cn

[Q63] 开启事务
来源：http://gjn.chenjidiqi.icu

START TRANSACTION;                -- 或 BEGIN
来源：http://hbq.fengsongda.top

[Q64] 提交事务
来源：http://zzy.wangdashe.top

COMMIT;
来源：http://mgb.yj20258.top

[Q65] 回滚事务
来源：http://nbh.yonumen.top

ROLLBACK;
来源：http://bih.cucudq.cn

[Q66] 行锁查询
来源：http://ugc.yueranfly.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qte.gzhubu.top

[Q67] 设置隔离级别
来源：http://bfv.zdqjudy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kpy.cqqwz.cn

[Q68] 保存点
来源：http://gbf.dianchejie.cn

SAVEPOINT sp1;
来源：http://ifx.chenjidiqi.icu

ROLLBACK TO sp1;
来源：http://ypb.xuetiantiany.cn

[Q69] 查看执行计划
来源：http://oax.xinyue.icu

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mta.zdqjudy.top

[Q70] 更新统计信息
来源：http://ltc.smart0.xyz

ANALYZE TABLE users;
来源：http://hui.aizwys.cn

[Q71] 查看建表语句
来源：http://twm.zdqjudy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://esd.yj202588.top

[Q72] 查看索引
来源：http://wiv.hesvh.cn

SHOW INDEX FROM users;
来源：http://rfd.haohaochexian.top

[Q73] 查看表状态
来源：http://bfw.dianchejie.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rfl.dianchejie.cn

[Q74] 强制使用索引
来源：http://owg.fanxiaobao.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://scg.pycfn.com

[Q75] 日期格式化
来源：http://zsp.tanke756.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ofq.cucudq.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://myo.cashguo.top

[Q76] 按天统计
来源：http://fxm.9152youxi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vwk.uphjek.com

[Q77] 时间加减
来源：http://dej.zhengqikj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tnj.yj20258.top

[Q78] 当前时间
来源：http://pex.redwolf501.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nuu.fanxiaobao.xyz

[Q79] 字符串拼接
来源：http://rqk.tarul.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gzt.nanxinkj.top

[Q80] 字符串截取
来源：http://doa.xinyue.icu

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qck.quarkkingdee.top

[Q81] 字符串替换
来源：http://urf.guannengcc.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rew.ctjpmb.com

[Q82] 字符长度与字节长度
来源：http://uie.quarkkingdee.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://btk.guannengcc.top

[Q83] 大小写转换
来源：http://xmg.yonumen.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://meu.shanyushiyangkeji.top

[Q84] 去除首尾空格
来源：http://kac.52xcode.cn

SELECT TRIM(name) FROM users;
来源：http://uzb.ivvv.top

[Q85] 数值取整
来源：http://bqq.hywenlv.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kuw.smart0.xyz

[Q86] 读取 JSON 字段
来源：http://hll.daxiang520.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fjr.hywenlv.cn

[Q87] JSON 字段做条件
来源：http://cmx.shanyushiyangkeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fnc.svipenyu.cn

[Q88] 行转列（条件聚合）
来源：http://exa.havefunace.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wqp.chenlongwang.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yfp.birdmap.top

[Q89] 判断表是否存在
来源：http://lkm.xuetiantiany.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://imj.feifeiyinyue.top

[Q90] 生成序号列
来源：http://opt.52xcode.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://obl.nanxinkj.top

================================================================================
来源：http://xrg.jlsjyb.cn

R. Bash 专题
来源：http://nnz.yanxiufei.cn

================================================================================
来源：http://ids.ehwqpu.com

[R01] shebang 与严格模式
来源：http://ora.yfazqb.com

#!/usr/bin/env bash
来源：http://oyk.yueranfly.top

set -euo pipefail
来源：http://arg.hnxiangtu.top

[R02] 变量赋值与使用
来源：http://upb.yj20258888.top

name="Tom"; echo "$name"
来源：http://uio.xziqi.cn

[R03] 只读变量
来源：http://kaj.tanke756.top

readonly PI=3.14
来源：http://ovj.xinyue.icu

[R04] 位置参数
来源：http://xsl.0kj1m.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://adh.xziqi.cn

[R05] 参数默认值
来源：http://uvh.cheryme.top

name="${1:-default}"
来源：http://ztw.jqgfzy.top

[R06] 判断命令是否存在
来源：http://orz.vehdjk.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gwx.tanke756.top

[R07] if 判断文件
来源：http://qwb.zdbjq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yej.hammf.cn

[R08] 数值比较
来源：http://avk.52xcode.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vag.0kj1m.cn

[R09] 字符串比较
来源：http://ttj.yonumen.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://awt.gogol.net.cn

[R10] 正则匹配
来源：http://zow.shanyushiyangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nap.daxiang520.top

[R11] case 多分支
来源：http://kys.zhiwuduotai.top

case "$1" in
来源：http://dso.jianghu66.top

start) echo "启动" ;;
来源：http://ajl.fengsongda.top

stop)  echo "停止" ;;
来源：http://jlx.fktsv.cn

*)     echo "未知命令" ;;
来源：http://aoa.epnwcf.com

esac
来源：http://ftg.shangyingyoupin.top

[R12] for 遍历文件
来源：http://iin.ppjwa.cn

for f in *.txt; do echo "$f"; done
来源：http://eqn.birdmap.top

[R13] for 计数循环
来源：http://crk.fengsongda.top

for i in {1..10}; do echo "$i"; done
来源：http://jdk.52xcode.cn

[R14] C 风格 for
来源：http://syf.hammf.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rbm.aibaodan.cn

[R15] while 逐行读文件
来源：http://uyb.wangdashe.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pqx.kuanghao11.cn

[R16] until 等待条件
来源：http://uho.jinqigufen.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ngo.tanke756.top

[R17] 数组定义与取值
来源：http://dep.tianlin.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://dhh.gogol.net.cn

[R18] 遍历数组
来源：http://zxr.jiagoushi.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gzr.feifeiyinyue.top

[R19] 数组长度
来源：http://nxn.fktsv.cn

echo "${#arr[@]}"
来源：http://rwh.hysaishi.cn

[R20] 关联数组（字典）
来源：http://tcp.jinqigufen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fze.ydjk.org.cn

[R21] 字符串长度
来源：http://gwg.jinqigfzy.top

echo "${#s}"
来源：http://dwc.sysykeji.top

[R22] 截取子串
来源：http://mby.yuxming.cn

echo "${s:0:5}"
来源：http://apo.shanyushiyangkeji.top

[R23] 字符串替换
来源：http://ugn.tian-w.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://emx.dashuyun.cn

[R24] 大小写转换
来源：http://kdp.ydzc1.top

echo "${s^^}"; echo "${s,,}"
来源：http://fyj.bjfxy.top

[R25] 去后缀 / 去前缀
来源：http://ioo.tarul.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hqw.ppjwa.cn

[R26] 命令替换
来源：http://wwt.fengsongda.top

now=$(date +%F); echo "$now"
来源：http://iic.jianghu66.top

[R27] 算术展开
来源：http://uzj.yj20258888.top

echo $((1 + 2 * 3))
来源：http://zgn.sxryk.cn

[R28] 浮点运算
来源：http://yjm.jinyuanbaomall.cn

echo "scale=2; 10/3" | bc
来源：http://gro.xuetiantiany.cn

[R29] 定义函数
来源：http://pge.daria6918.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vkx.xylfe.cn

[R30] 函数返回状态码
来源：http://hsr.snrcjt.cn

f() { return 0; }; f || echo "失败了"
来源：http://mce.tianlin.xyz

[R31] 局部变量
来源：http://uqk.fanxiaobao.xyz

f() { local x=1; echo "$x"; }
来源：http://rhu.nanxuanxn.top

[R32] 参数个数校验
来源：http://sny.wangshuangyany.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hwy.fengsongda.top

[R33] 捕获错误并提示行号
来源：http://nvq.daxiang520.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ejv.feifeiyinyue.top

[R34] 退出时清理
来源：http://fxz.jinqigfzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://jiz.jianghu66.top

[R35] 后台执行并等待
来源：http://gxb.hnqzz.top

sleep 5 & pid=$!; wait "$pid"
来源：http://hld.guowangkeji.top

[R36] 并发执行多个任务
来源：http://uau.chenlongwang.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://syd.feifeiyinyue.top

[R37] 把输出赋给变量
来源：http://nql.hywenlv.cn

files=$(ls -1)
来源：http://vco.birdmap.top

[R38] 管道串联
来源：http://vvh.jlsjyb.cn

cat a.txt | grep -i error | wc -l
来源：http://mip.yueranfly.top

[R39] 重定向标准输出与错误
来源：http://okz.yueranfly.top

cmd > out.log 2>&1
来源：http://dxu.ehwqpu.com

[R40] 追加写日志
来源：http://txe.sjlbkw.cn

echo "log" >> out.log
来源：http://wny.vqdsnc.cn

[R41] 丢弃输出
来源：http://shu.hywenlv.cn

cmd >/dev/null 2>&1
来源：http://exp.yfazqb.com

[R42] 输入重定向
来源：http://ckq.chenzaomai.com

wc -l < a.txt
来源：http://qbr.vehdjk.com

[R43] 按名字查找文件
来源：http://xku.zdbjq.cn

find . -name "*.log" -type f
来源：http://gqb.fanxiaobao.xyz

[R44] 按修改时间查找
来源：http://rvo.yuxming.cn

find . -mtime -7 -type f
来源：http://bpp.meibo888.top

[R45] 批量删除
来源：http://bnk.52xcode.cn

find . -name "*.tmp" -delete
来源：http://pem.shzxlz.cn

[R46] 递归替换文件内容
来源：http://mbk.yonumen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cxf.yj202588.top

[R47] sed 单行替换
来源：http://jvb.cdnleiting.top

sed -i 's/foo/bar/g' a.txt
来源：http://fsh.gzhubu.top

[R48] awk 取指定列
来源：http://xcr.jiagoushi.top

awk '{print $1, $3}' a.txt
来源：http://kkf.guowangkeji.top

[R49] awk 带条件
来源：http://eyp.jyoumei.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rkx.xylfe.cn

[R50] awk 求和
来源：http://lgh.dashuyun.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dsf.bjfxy.top

[R51] 排序去重取前几
来源：http://jpz.tian-w.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ysa.chenjidiqi.icu

[R52] 统计行数
来源：http://dja.hongshengwenyu.top

wc -l a.txt
来源：http://rgg.shzxlz.cn

[R53] 查看文件头与实时尾
来源：http://niv.nanxinkj.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mdg.zhoulong.xyz

[R54] 比较两个文件
来源：http://ort.yuxming.cn

diff a.txt b.txt
来源：http://qfc.jinyuanbaomall.cn

[R55] 压缩与解压
来源：http://ubc.wangdashe.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qlo.nanxinkj.top

[R56] 远程拷贝
来源：http://qlx.ydzc1.top

scp file user@host:/path/
来源：http://xgs.yj20258888.top

[R57] 远程执行命令
来源：http://mdt.shanyushiyangkeji.top

ssh user@host 'uptime'
来源：http://fbg.jianghu66.top

[R58] 下载文件
来源：http://psr.yj202588.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xtn.sysykeji.top

[R59] 发 POST JSON
来源：http://uqq.xuetiantiany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nhw.aibaodan.cn

[R60] 只看 HTTP 状态码
来源：http://nmx.cashguo.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ocs.snrcjt.cn

[R61] 磁盘占用
来源：http://wvb.zhongyouzk.top

df -h;  du -sh *
来源：http://emt.pengpengdd.cyou

[R62] 找最占空间的文件
来源：http://gry.nanxuanxn.top

du -ah . | sort -rh | head -10
来源：http://tcv.jinghuilouyu.cn

[R63] 内存与进程
来源：http://otp.gzhubu.top

free -h;  ps aux | grep nginx
来源：http://rnb.daria6918.cn

[R64] 结束进程
来源：http://qof.wangdashe.top

kill -9 $(pgrep -f app.py)
来源：http://hjk.shanyushiyangkeji.top

[R65] 查看端口占用
来源：http://yms.hysaishi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rjj.tarul.cn

[R66] 定时任务
来源：http://igh.ydjk.org.cn

crontab -e;  crontab -l
来源：http://ypx.bbcook.cn

[R67] 生成随机十六进制串
来源：http://wme.yonumen.top

openssl rand -hex 16
来源：http://wcj.jiagoushi.top

[R68] 计算文件校验值
来源：http://tmf.yuxming.cn

sha256sum a.txt;  md5sum a.txt
来源：http://joe.shuidangran.top

[R69] 生成随机密码
来源：http://cuu.ydjk.org.cn

head -c 16 /dev/urandom | base64
来源：http://zix.vehdjk.com

[R70] 时间戳与互转
来源：http://xui.pycfn.com

date +%s;  date -d @1700000000
来源：http://xdb.zdbjq.cn

[R71] 日期格式化
来源：http://quu.chenlongwang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://anu.birdmap.top

[R72] 等待端口就绪
来源：http://aur.zhengqikj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://axd.yj20258.top

[R73] 分割大日志
来源：http://vim.xylfe.cn

split -l 1000 big.log part_
来源：http://mph.jinqigufen.top

[R74] 批量重命名
来源：http://koq.jlsjyb.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cch.hywenlv.cn

[R75] 导出环境变量
来源：http://ssv.uphjek.com

export PATH="$HOME/bin:$PATH"
来源：http://eay.gzhubu.top

[R76] 使用临时文件
来源：http://jwh.ydjk.org.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rdt.zhiwuduotai.top

[R77] 读取用户输入
来源：http://zua.chenlongwang.top

read -rp "请输入: " ans
来源：http://vmv.nwbrower.top

[R78] 交互式菜单
来源：http://wcm.fzhhl.top

select opt in a b c; do echo "$opt"; break; done
来源：http://pkp.havefunace.top

[R79] 解析命令行选项
来源：http://ymw.hesvh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rlq.sweek.top

[R80] 查看脚本执行耗时
来源：http://rky.shzxlz.cn

time ./run.sh
来源：http://xse.wangdashe.top

================================================================================
来源：http://yvu.c1oappe.top

S. C / C++ 专题
来源：http://rcc.epnwcf.com

================================================================================
来源：http://xzu.cdnleiting.top

[S01] C：Hello World
来源：http://bfb.daria6918.cn

#include <stdio.h>
来源：http://mvy.jinqigfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://fwz.fktsv.cn

[S02] C：变量与格式化输出
来源：http://gfc.tarul.cn

int a = 10; printf("%d\n", a);
来源：http://rcm.andypj.xyz

[S03] C：读入整数
来源：http://sdl.nanxinkj.top

int x; scanf("%d", &x);
来源：http://ajl.quarkkingdee.top

[S04] C：字符串复制
来源：http://qvb.sjlbkw.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cux.xylfe.cn

[S05] C：字符串长度
来源：http://ret.hywenlv.cn

strlen(s)
来源：http://few.nanxuanxn.top

[S06] C：字符串比较
来源：http://wic.jqgufenzy.top

strcmp(a, b) == 0
来源：http://cdu.cucudq.cn

[S07] C：数组遍历求和
来源：http://mpa.bbcook.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://aut.jlsjyb.cn

[S08] C：动态内存分配与释放
来源：http://vjh.yj20258.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dwl.fehbvm.com

[S09] C：结构体定义与初始化
来源：http://eeq.shanyushiyangtech.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cox.c1oappe.top

[S10] C：指针与解引用
来源：http://rqa.yonumen.top

int *p = &a;  *p = 5;
来源：http://uzf.haohaochexian.top

[S11] C：逐行读文件
来源：http://shz.zdbjq.cn

FILE *f = fopen("a.txt", "r");
来源：http://xnl.mhx1999.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://mxo.dashuyun.cn

fclose(f);
来源：http://zyj.jqgufenzy.top

[S12] C：写文件
来源：http://epl.ywan-chungtsiang.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gbh.iojbl.cn

[S13] C：宏定义
来源：http://gax.zhoulong.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xiu.quarkkingdee.top

[S14] C：枚举
来源：http://lgy.birdmap.top

enum Color { RED, GREEN, BLUE };
来源：http://ogt.wangdashe.top

[S15] C：类型转换
来源：http://ylh.sysykeji.top

(double) a / b
来源：http://kbu.iojbl.cn

[S16] C：位操作置位
来源：http://ulq.feifeiyinyue.top

x |= (1 << 3);
来源：http://hxh.hongshengwenyu.top

[S17] C：安全拼接字符串
来源：http://cxq.zhoulong.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bcj.shanyushiyangtech.top

[S18] C：命令行参数
来源：http://yuq.xuanzx.com

int main(int argc, char **argv)
来源：http://egd.0kj1m.cn

[S19] C：快速排序
来源：http://rcv.yueranfly.top

qsort(a, n, sizeof(int), cmp);
来源：http://gve.dashuyun.cn

[S20] C：二分查找
来源：http://xjz.ehwqpu.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jxh.chenjidiqi.icu

[S21] C：字符类别判断
来源：http://jua.bbcook.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://izc.havefunace.top

[S22] C：字符串转数字
来源：http://zny.hnqzz.top

atoi("42");  strtod("3.14", NULL);
来源：http://iwo.uphjek.com

[S23] C：随机数
来源：http://avb.hfpthk.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nmn.c1oappe.top

[S24] C：获取本地时间
来源：http://hle.316326.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gol.jlsjyb.cn

[S25] C：内存拷贝
来源：http://mni.cheryme.top

memcpy(dst, src, n);
来源：http://kzt.gogol.net.cn

[S26] C：内存清零
来源：http://hye.yueranfly.top

memset(a, 0, sizeof a);
来源：http://onb.gotoacloud.top

[S27] C：定义常量
来源：http://wda.kuanghao11.cn

const double PI = 3.14159;
来源：http://kln.havefunace.top

[S28] C：静态变量
来源：http://clw.birdmap.top

static int counter = 0;
来源：http://qmd.uphjek.com

[S29] C：变参函数
来源：http://qpz.tian-w.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://iny.dianchejie.cn

[S30] C：头文件保护
来源：http://ryf.pengpengdd.cyou


<!-- 参考信息 -->